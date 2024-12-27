<body>
	<div id="page">
		<h1>Noe's Points <span>🩵</span></h1>
		<div id="quackContainer">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				id="quackPath"
				viewBox="0 0 600 600"
				preserveAspectRatio="xMidYMid meet"
			>
				<g transform="translate(0,600) scale(0.1,-0.1)"  stroke="none">
					<path
						d="M2534 4765 c-265 -47 -496 -197 -694 -453 -19 -24 -45 -39 -96 -57
            -111 -39 -203 -49 -307 -35 -85 12 -90 11 -134 -12 -133 -68 -104 -258 68
            -442 174 -186 392 -274 572 -232 159 37 230 116 206 228 -11 49 -37 90 -121
            196 -105 133 -110 160 -45 248 145 196 325 324 528 375 118 30 302 24 407 -14
            315 -111 473 -398 408 -740 -29 -149 -103 -276 -262 -447 -53 -58 -106 -118
            -116 -135 -27 -45 -23 -91 10 -125 38 -37 96 -45 337 -45 210 0 327 18 501 74
            193 63 426 184 604 314 41 31 78 52 81 49 11 -12 68 -242 90 -367 30 -170 38
            -487 15 -643 -48 -323 -204 -603 -440 -786 -196 -153 -423 -248 -706 -297
            -621 -107 -1362 115 -1671 499 -68 84 -130 204 -154 297 -22 87 -19 234 6 336
            46 180 136 333 293 498 132 139 166 185 166 226 0 45 -41 85 -88 85 -30 0 -43
            -9 -101 -72 -36 -40 -101 -110 -145 -157 -296 -318 -402 -737 -269 -1069 55
            -138 158 -281 282 -390 422 -372 1148 -536 1797 -407 339 68 642 227 845 443
            409 435 491 1087 238 1905 -53 173 -95 187 -230 80 -268 -212 -571 -364 -830
            -417 -100 -21 -282 -36 -341 -29 l-47 5 63 72 c159 183 230 332 256 540 53
            418 -188 783 -585 886 -105 28 -282 34 -391 15z m-754 -748 c17 -45 66 -118
            152 -226 40 -50 41 -54 24 -67 -25 -18 -98 -28 -154 -20 -114 15 -277 132
            -361 257 -23 34 -41 65 -41 70 0 4 51 8 113 8 61 1 139 7 172 15 33 7 64 13
            69 12 4 -1 16 -23 26 -49z"
					/>
					<path
						d="M2381 4212 c-52 -26 -75 -63 -75 -121 0 -119 133 -181 224 -105 76
            65 57 191 -36 230 -44 18 -72 18 -113 -4z"
					/>
				</g>
			</svg>
			<div id="quackProgressForm">
				<div id="quackProgress"></div>
			</div>
		</div>
		<span id="points"> 97/300 </span>
	</div>
</body>

<script>
	import { onMount } from "svelte";

    onMount(() => {
       const quackProgress = document.getElementById("quackProgress")
       if (quackProgress) {
        setTimeout(() => {
                quackProgress.style.height = '55%';
            }, 50);
       }
    })
</script>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Playwrite+HU&family=Playwrite+PL+Guides&display=swap');

	body {
		padding-top: 50px;
		margin: 0;
		width: 100%;
		height: 100%;
		background-color: #242424;
	}
    span{
        text-shadow: none;
    }
	h1 {
		font-family: 'Playwrite HU';
        font-size: 300%;
        animation: pulsate 0.2s ease-in-out infinite alternate;
        color: #fff;
		text-shadow:
			0 0 7px #fff,
			0 0 10px #fff,
			0 0 21px #fff,
			0 0 42px #f09,
			0 0 82px #f09,
			0 0 92px #f09,
			0 0 102px #f09,
			0 0 151px #f09;
	}

    @keyframes pulsate {
    
    100% {
  
        text-shadow:
        0 0 4px #fff,
        0 0 11px #fff,
        0 0 19px #fff,
        0 0 40px #f09,
        0 0 80px #f09,
        0 0 90px #f09,
        0 0 100px #f09,
        0 0 150px #f09;
    
    }
    
    0% {
  
      text-shadow:
      0 0 4px #fff,
      0 0 10px #fff,
      0 0 18px #fff,
      0 0 38px #f09,
      0 0 73px #f09,
      0 0 80px #f09,
      0 0 94px #f09,
      0 0 140px #f09;
  
  }
}

	#points {
        margin-top: -80px;
        font-size: 70px;
        font-weight: bold;
		font-family: 'Playwrite HU';
	}
	#page {
		width: 100%;
		min-width: 100%;
		min-height: 100%;
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	#quackProgress {
		width: 100%;
		height: 0%;
		position: absolute;
		bottom: 0;
		background-color: yellow;
        transition: height 2.5s ease-out;
	}
	#quackProgressForm {
		position: absolute;
		top: 118px;
		left: 130px;
		width: 100%;
		height: 100%;
		clip-path: path(
			'M322.6,112.66c6.81,1.96,9.5,10.88,13.18,23.66,3.27,11.39,9.33,37.7,2.85,83.76-2.02,14.4-3.44,24.05-7.96,36.88-4.46,12.63-11.1,31.46-28.51,47.2-10.63,9.61-21.82,15.31-30.7,19.28-7.63,3.4-16.17,6.55-23.81,9.27-27.94,10.58-66.51,18.49-103.06,10.85-15.22-2.89-28.91-8.15-42.88-14.36-21.21-9.81-42.75-18.35-58.34-35.75-5.52-6.17-14.6-16.91-19.29-33.35-7.38-25.89-1.03-56.61,15.3-77.51,11.19-14.32,20.89-16.14,29.14-34.22,1.92-4.21,10.44-22.88,3.09-31.07-5-5.57-12.38-.76-28.43-6.06-3.88-1.28-12.83-4.66-21.09-11.89-1.3-1.14-22.06-19.64-17.41-31.58,5.18-13.3,35.8,1.12,56.67-20.26,16.22-16.62,19.41-26,42.52-35.92,17.68-7.51,41.57-10.75,59.6-3.56,58.73,24.34,65.35,85.91,23.21,129.89-18.63,20.98,6.8,25.1,27.23,23.16,8.13-.77,14.7-1.58,20.24-2.9,10.22-2.45,27.66-6.62,46.89-18.01,26.2-15.51,31.88-30.27,41.55-27.49Z'
		);
	}
	#quackContainer {
		align-items: center;
		align-content: center;
		position: relative;
		width: 600px;
		height: 600px;
		display: flex;
		justify-content: center;
		align-items: center;
	}

	#quackPath {
        fill: #000000;
        
		z-index: 1;
		width: 100%;
		height: 100%;
	}
</style>
