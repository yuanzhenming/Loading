<template>
	<div class="loader">
        <div class="loader-inner ball-clip-rotate">
          <div></div>
        </div>
     </div>
</template>

<script>
	export default {
		data() {
			return {
				mes: 'Loading...*^_^*'
			}
		}
	}
</script>

<style scoped>
	.loader {
		width: 30px;
		height: 30px;
		margin: 50px auto;
		text-align:center;
	}
	@keyframes rotate {
	  0% {
			    -webkit-transform: rotate(0deg) scale(1);
			    transform: rotate(0deg) scale(1);
	     }

	  50% {
		   		-webkit-transform: rotate(180deg) scale(0.6);
		        transform: rotate(180deg) scale(0.6); 
	      }

	  100% {
		    	-webkit-transform: rotate(360deg) scale(1);
		        transform: rotate(360deg) scale(1); 
	       } 
    }

.ball-clip-rotate > div {
  background-color: #f60;
  width: 15px;
  height: 15px;
  border-radius: 100%;
  margin: 2px;
  -webkit-animation-fill-mode: both;
          animation-fill-mode: both;
  border: 2px solid #f60;
  border-bottom-color: transparent;
  height: 25px;
  width: 25px;
  background: transparent !important;
  display: inline-block;
  -webkit-animation: rotate 0.75s 0s linear infinite;
  animation: rotate 0.75s 0s linear infinite; 
  }

	
</style>