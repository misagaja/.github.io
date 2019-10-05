<!DOCTYPE html>
<center><h1 ><span id="naslov">ovde bi trebalo da dodje</span></h1><br>

<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script> 
flag=1;
$(window).scroll(function(){$('#div1').each(function(){if(isScrolledIntoView($(this))){$(this).children('span').text('visible');if(flag){setaj();flag=0;}}else{$(this).children('span').text('invisible');flag=1;}});});

function isScrolledIntoView(elem){var $elem = $(elem);
    var $window = $(window);

    var docViewTop = $window.scrollTop();
    var docViewBottom = docViewTop + $window.height();

    var elemTop = $elem.offset().top;
    var elemBottom = elemTop + $elem.height();

    return ((elemBottom <= docViewBottom) && (elemTop >= docViewTop));}function setaj(){var div = $("#div1");
    div.animate({left: '300px', opacity: '0.99'}, "slow","swing");
    div.animate({left: '-250px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '250px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '-150px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '200px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '-100px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '150px', opacity: '0.9'}, "fast","swing");
    div.animate({left: '-50px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '50px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '-20px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '20px', opacity: '0.9'}, "fast","swing");
    div.animate({left: '-10px', opacity: '0.99'}, "fast","swing");
    div.animate({left: '10px', opacity: '0.99'}, "fast","swing");};

</script> 
<style>
    #heart {
      position: relative;
      width: 100px;
      height: 90px;
	
    }
    #heart:before,
    #heart:after {
      position: absolute;
      content: "";
      left: 50px;
      top: 0;
      width: 50px;
      height: 80px;
 background-image: url("https://cdn.bitrix24.site/bitrix/images/landing/business/560x560/img6.jpg");
//background: url(http://mammy.rs/wp-content/uploads/2018/12/mammy2.jpg); 
background-size:     cover;      
//background: red;
      border-radius: 50px 50px 0 0;
      transform: rotate(-45deg);
      transform-origin: 0 100%;
    }
    #heart:after {
      left: 0;
      transform: rotate(45deg);
      transform-origin: 100% 100%;
    }

   #hexagon {
      width: 100px;
      height: 55px;
      background: red;
      position: relative;


    }
    #hexagon:before {
      content: "";
      position: absolute;
      top: -25px;
      left: 0;
      width: 0;
      height: 0;
      border-left: 50px solid transparent;
      border-right: 50px solid transparent;
      border-bottom: 25px solid red;
    }
    #hexagon:after {
      content: "";
      position: absolute;
      bottom: -25px;
      left: 0;
      width: 0;
      height: 0;
      border-left: 50px solid transparent;
      border-right: 50px solid transparent;
      border-top: 25px solid red;
 background-image: url("http://mammy.rs/wp-content/uploads/2018/12/mammy2.jpg");

background-size:     cover;    
    }
  
#sl {
	 width: 100px;
      height: 90px;
}  
svg{
  width:30%;
position:relative;float:left;
left:0px;
}
#div2 {position:relative;left:200px;top:-100px;display:block-inline;transition: all 3s;}
#div2:hover {left:-100px;top:-200px;}
#sl5 {position:relative;left:0px;top:0px;display:block-inline;transition: all 3s;}
#sl5:hover {left:100px;top:-200px;}
</style>

</head>

<body>






<div>
<svg  viewBox="0 0 100 100" version="1.1" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="img" patternUnits="userSpaceOnUse" width="100" height="100">
 <image xlink:href="https://cdn.bitrix24.site/bitrix/images/landing/business/560x560/img6.jpg" x="-25" width="150" height="100" />

    </pattern>
  </defs>
<!--<polygon points="50 1 95 25 95 75 50 99 5 75 5 25" fill="url(#img)"/>-->
  <polygon points="50 1 95 25 95 75 50 99 5 75 5 25" fill="url(#img)"/>
</svg>

<svg viewBox="0 0 100 100" version="1.1" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="img1" patternUnits="userSpaceOnUse" width="100" height="100">
      <image xlink:href="https://farm4.staticflickr.com/3165/5733278274_2626612c70.jpg" x="-25" width="150" height="100" />
 
    </pattern>
  </defs>
  <polygon points="50 1 95 25 95 75 50 99 5 75 5 25" fill="url(#img1)"/>
</svg>
<svg viewBox="0 0 100 100" version="1.1" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="img2" patternUnits="userSpaceOnUse" width="100" height="100">
 <image xlink:href="http://mammy.rs/wp-content/uploads/2018/12/mammy2.jpg" x="-25" width="150" height="100" />

    </pattern>
  </defs>
  <polygon points="50 1 95 25 95 75 50 99 5 75 5 25" fill="url(#img2)"/>
</svg>
</div>
<div id="div2" style="">
<svg  viewBox="0 0 100 100" version="1.1" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="img" patternUnits="userSpaceOnUse" width="100" height="100">
 <image xlink:href="https://cdn.bitrix24.site/bitrix/images/landing/business/560x560/img6.jpg" x="-25" width="150" height="100" />

    </pattern>
  </defs>
  <polygon points="50 1 95 25 95 75 50 99 5 75 5 25" fill="url(#img)"/>
</svg>

<svg id="sl5" viewBox="0 0 100 100" version="1.1" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="img5" patternUnits="userSpaceOnUse" width="100" height="100">
      <image  xlink:href="https://lh3.googleusercontent.com/-jlWnLvic3io/AAAAAAAAAAI/AAAAAAAAAAA/ACHi3reVzg3gWJmVzOlrzoye_Lbq19bGNQ/s48-c-mo/photo.jpg" x="-25" width="150" height="100" />
 
    </pattern>
  </defs>
  <polygon points="50,1 95,25 95,75 50,99 5,75 5,25" fill="url(#img5)"/>
</svg>
<svg viewBox="0 0 100 100" version="1.1" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="img2" patternUnits="userSpaceOnUse" width="100" height="100">
 <image xlink:href="http://mammy.rs/wp-content/uploads/2018/12/mammy2.jpg" x="-25" width="150" height="100" />

    </pattern>
  </defs>
  <polygon points="50 1 95 25 95 75 50 99 5 75 5 25" fill="url(#img2)"/>
</svg>
<svg height="450" width="400">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />

</svg>
<svg height="150" width="500">
  <defs>
    <radialGradient id="grad2" cx="50%" cy="50%" r="50%" fx="50%" fy="50%">
      <stop offset="0%" style="stop-color:rgb(255,255,255);
      stop-opacity:0" />
      <stop offset="100%" style="stop-color:rgb(0,0,255);stop-opacity:1" />
    </radialGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad2)" />
</svg>
<svg height="150" width="400">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad1)" />
</svg>
<svg height="150" width="500">
  <defs>
    <radialGradient id="grad2" cx="50%" cy="50%" r="50%" fx="50%" fy="50%">
      <stop offset="0%" style="stop-color:rgb(255,255,255);
      stop-opacity:0" />
      <stop offset="100%" style="stop-color:rgb(0,0,255);stop-opacity:1" />
    </radialGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad2)" />
</svg>
</div>
<div style="position:relative;float:left;clear:left;">
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>
aaaaaaaaaaaaaaa<br>aaaaaaaaaaaaaaa<br>
</div>
</body>
</html>
