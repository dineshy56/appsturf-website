# appsturf-website
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
  <title>Appsturf | Mobile application development company</title>
  <meta name="description" content="Appsturf Technologies Pvt Ltd">
  <link rel="icon" type="image/png" href="images/work/faviconicon.png">

  <link href="style/style.css" rel="stylesheet" type="text/css">
  <link href="style/responsive.css" rel="stylesheet" type="text/css">
  <link rel="stylesheet" type="text/css" href="style/aboutstyle.css">
  <link rel="stylesheet" type="text/css" href="style/responsiveabout.css">
  <link rel="stylesheet" type="text/css" href="css/demo.css" />
  <link rel="stylesheet" type="text/css" href="css/style1.css" />
 
  <script type="text/javascript" src="script/modernizr.custom.86080.js"></script>
  <script async="" src="script/analytics.js"></script>
  <script type="text/javascript" src="script/jquery-2.1.1.min.js"></script>
  <script src="https://code.jquery.com/jquery-2.0.3.min.js"></script>
  <script src="https://prinzhorn.github.io/skrollr/dist/skrollr.min.js"></script>

<!-- ----top logo scroll and scale---- -->
  <link rel="stylesheet" href="style/scrollcss/css/scroll.css" type="text/css">
  <script type="text/javascript" src="style/scrollcss/script/js/lib/greensock/TweenMax.min.js"></script>
  <script type="text/javascript" src="style/scrollcss/script/scrollmagic/uncompressed/ScrollMagic.js"></script>
  <script type="text/javascript" src="style/scrollcss/script/scrollmagic/uncompressed/plugins/animation.gsap.js"></script>
  <script type="text/javascript" src="style/scrollcss/script/scrollmagic/uncompressed/plugins/debug.addIndicators.js"></script>
</head>
<!-- ==============top headder ============ -->
<script type="text/javascript">
  function sticky_relocate() {
    var window_top = $(window).scrollTop();
    var div_top = $('#sticky-anchor').offset().top;
    if (window_top > div_top) {
        $('#sticky').addClass('stick');
        $('#sticky-anchor').height($('#sticky').outerHeight());
    } else {
        $('#sticky').removeClass('stick');
        $('#sticky-anchor').height(0);
    }
}

$(function() {
    $(window).scroll(sticky_relocate);
    sticky_relocate();
});

var dir = 1;
var MIN_TOP = 200;
var MAX_TOP = 350;

function autoscroll() {
    var window_top = $(window).scrollTop() + dir;
    if (window_top >= MAX_TOP) {
        window_top = MAX_TOP;
        dir = -1;
    } else if (window_top <= MIN_TOP) {
        window_top = MIN_TOP;
        dir = 1;
    }
    $(window).scrollTop(window_top);
    window.setTimeout(autoscroll, 100);
}
</script>
<!-- ===preloader== -->
<script type="text/javascript">
  $(window).on('load', function() { // makes sure the whole site is loaded 
  $('#status').fadeOut(); // will first fade out the loading animation 
  $('#preloader').delay(0).fadeOut('slow'); // will fade out the white DIV that covers the website. 
  $('body').delay(0).css({'overflow':'visible'});
})

</script>

<style type="text/css">

</style>
<body>
   <!-- -------------- loadder------------- -->
   <div id="preloader">
    <div id="status">&nbsp;</div>
  
        <div class="spinner">
            <div class="double-bounce1"></div>
            <div class="double-bounce2"></div>
          </div>
  </div>

    <!-- -------------- slider images------------- -->
  <div class="homeHolder">  
    <ul class="cb-slideshow">
      <li><span>Image 01</span><div><h3 class="sliderH3">Mobile Apps</h3></div></li>
      <li><span>Image 02</span><div><h3 class="sliderH3">Web Apps</h3></div></li>
      <li><span>Image 03</span><div><h3 class="sliderH3"> We are hiring </h3></div></li>
      <li><span>Image 04</span><div><h3 class="sliderH3">Mobile Apps </h3></div></li>
      <li><span>Image 05</span><div><h3 class="sliderH3">Web Apps</h3></div></li>
      <li><span>Image 06</span><div><h3 class="sliderH3">We are hiring</h3></div></li>
    </ul>
    <div class="navnew" id="myTopnav">	
    	<div class="screen">
            <div class="circle"></div>
            <div class="menuburger">
              <ul class="burgerUL">
                <li class="burgerLI"><a href="home.html" >Home</a></li>
                <li class="burgerLI"><a href="work.html" >Works</a></li>
                <li class="burgerLI"><a href="about.html" class="newlmink ">About</a></li>
                <li class="burgerLI"> <a href="contact.html" class="newmlink active">Contact</a></li>
                        
              </ul>
            </div>                  
            <div class="burger">
              <div class="navBAAR">
              <div class="x"></div>
              <div class="y"></div>
              <div class="z"></div>
              </div>
            </div>    
      </div>
    </div>

<!-- <div id="openmenu"></div> -->
    <nav style="top: 80%;" class="">
       <a href="home.html"><div class="menu menublog"><span class="number">01</span><span class="label">Home</span></div></a>
       <a href="work.html"><div class="menu menuworks"><span class="number">02</span><span class="label">Works</span></div></a>
      <a href="about.html"><div class="menu menuabout"><span class="number">03</span><span class="label">About</span></div></a>
       <a href="contact.html"><div class="menu menucontact"><span class="number">04</span><span class="label">Contact</span></div></a>
    </nav>

    <section class="demo">
      <div class="centerLogo">
            <div class="spacer s1"></div>
            <div id="trigger2"></div>
            <div id="animate2">
            	 <a href="home.html"> <img src="images/work/appsturfhomelogo.png" class="imgClass">  </a>
            </div>
      </div>
          <script>
                  var controller = new ScrollMagic.Controller({
                globalSceneOptions: {
                  triggerHook: '0.4'
                }
              });
            // build scene
            var scene = new ScrollMagic.Scene({triggerElement: "#trigger2", offset:70,duration: 800})
                    // animate color and top border in relation to scroll position
                    .setTween("#animate2", {scale: 0.6})
                    // the tween durtion can be omitted and defaults to 1
                    /*.addIndicators()*/ // add indicators (requires plugin)
                    .addTo(controller);
          </script>
          <script>
          var controller = new ScrollMagic.Controller({
                globalSceneOptions: {
                  triggerHook: '0.01 '
                }
              });
            $(function () { // wait for document ready
              // build scene
              var scene = new ScrollMagic.Scene({triggerElement: "#trigger2"})
                      .setPin("#animate2")
                     /* .addIndicators({name: "2 (duration: 0)"})*/ // add indicators (requires plugin)
                      .addTo(controller);
            });
          </script>
    </section>
    <div>
        <img src="images/work/mobilelogo.jpg" class="mobileLogo">
    </div>
    <section id="grid"  class="">
      <div>
        <div id="sticky-anchor"></div>
        <div id="sticky" class="pfix"><!-- <img src="logo.jpg"> --></div>
      </div>  
  	  <div class="introAbout">
        <h1 class="hometagline">We are Appsturf</h1>
        <p>&nbsp;Appsturf technologies is a digital solutions boutique located in Mumbai.<br>Appsturf has a diverse and far-reaching client base
          and portfolio with national and international clients.</br></p> 
      </div>
      <div class="introHR">
        <hr class="line">
        <h2>Our Recent Work</h2>      
      </div>      
    
      <div class="contentNew">
        <div class="faarbetter">
            <div class="textContentFB">
              <h2 class="fontStyleh2">Happy2Refer</h2>
              <div class="smallText"><hr class="hrClass"></hr>&nbsp;Android & iOS</div>
            </div>
            <div class="imgContentFB">
              <img src="images/homepageSnap/4.jpg" class="screenShot">
            </div>
            <div class="descriptionContentFB">
              <p class="descriptiontext">Happy2Refer app allows employees to view jobs open for referrals. It syncs your social media accounts to help you refer friends with a single...</p>
              <a href="project.html?workId=7"><button class="DISCOVER">DISCOVER</button></a>
            </div>
        </div>
        
        <div class="FYITV18">
            <div class="textContentFT">
              <h2 class="fontStyleh2">FYITV18</h2>
              <div class="smallText"><hr class="hrClass"></hr>&nbsp; Website</div>
            </div>
            <div class="imgContentFT">
              <img src="images/homepageSnap/newfyitv18.png" class="screenShot">
            </div>
            <div class="descriptionContentFT">
              <p class="descriptiontext">FYI TV18 is a new channel for a new India. The channel consists of an amalgamation of home, food, and relationships at its core...</p>
              <a href="project.html?workId=1"><button class="DISCOVER">DISCOVER</button></a>
            </div>
        </div>
        
        
        <div class="faarbetter">
            <div class="textContentFB">
              <h2 class="fontStyleh2">Oorja</h2>
              <div class="smallText"><hr class="hrClass">&nbsp;&nbsp;Android </div>
            </div>
            <div class="imgContentFB">
              <img src="images/homepageSnap/oorja.png" class="screenShot">
            </div>
            <div class="descriptionContentFB">
              <p class="descriptiontext">Oorja is an B2B app for their customer (hotels) which uses their product( stoves).It provides current grocery item prices, according to ...</p>
              <a href="oorja.html"><button class="DISCOVER ">DISCOVER</button></a>
            </div>
          
        </div>
      
        <div class="FYITV18">
            <div class="textContentFT">
              <h2 class="fontStyleh2">faar better films</h2>
               <div class="smallText"><hr class="hrClass">&nbsp;&nbsp;Website</div>
            </div>
            <div class="imgContentFT">
              <img src="images/homepageSnap/faarbetter.png" class="screenShot">
            </div>
            <div class="descriptionContentFT">
              <p class="descriptiontext">Faar Better Films is a Production House based in Mumbai, India. Considering Innovation in Ideas, Ingenuity In Creating Concepts, Simplicity in ...</p>
             <a href="project.html?workId=6"><button class="DISCOVER">DISCOVER</button></a>
            </div>
        </div> 

        <div class="faarbetter">
            <div class="textContentFB">
              <h2 class="fontStyleh2">rockabyte</h2>
              <div class="smallText"><hr class="hrClass">&nbsp;&nbsp;Android & Ios</div>
            </div>
            <div class="imgContentFB">
              <img src="images/homepageSnap/rockabyte.png" class="screenShot">
            </div>
            <div class="descriptionContentFB">
              <p class="descriptiontext">Rockabyte is an entertainment app It's a unique interactive platform for every individual to promote them self
				in the eyes of the world ...</p>
              <a href="rockabyte.html"><button class="DISCOVER ">DISCOVER</button></a>
            </div>
          
        </div>

        <div class="FYITV18">
            <div class="textContentFT">
              <h2 class="fontStyleh2">fusedcow</h2>
               <div class="smallText"><hr class="hrClass">&nbsp;&nbsp;ERP Tool</div>
            </div>
            <div class="imgContentFT">
              <img src="images/homepageSnap/fusedcow.png" class="screenShot">
            </div>
            <div class="descriptionContentFT">
              <p class="descriptiontext">Faar Better Films is a Production House based in Mumbai, India. Considering Innovation in Ideas, Ingenuity In Creating Concepts, Simplicity in ...</p>
             <a href="fusedcow.html"><button class="DISCOVER">DISCOVER</button></a>
            </div>
        </div> 

        <div class="newFooter">
              <div class="content">
                <div id="footerleft"> <span>BE SOCIAL WITH US</span><br>
                  <ul class="social-icons">
                     <li><a href="https://www.facebook.com/appsturf" target="_blank" ><img src="images/work/fb.png" class="homeicon hue-rotate"></a></li>
                      <li><a href="https://plus.google.com/106803749715716637707" target="_blank" ><img src="images/work/gp.png" class="homeicon hue-rotate"></a></li>
                      <li><a href="https://twitter.com/appsturf" target="_blank"><img src="images/work/tw.png" class="homeicon hue-rotate"></a></li>
                  </ul>
                </div>
                <div id="footerright"> <span>CONTACT</span> <strong>509, Spaces 912, Mira Bhayandar Rd,Pleasant Park, Mira Road East,</br>
                    Mumbai, Maharashtra 401107
                     </strong><br>
                    <a href="tel:+91 7709 805 786" class="homePhone"> +91 7709 805 786</a>,<a href="tel:+91 9665 006 351" class="homePhone">+91 9665 006 351</a>
                    <br>
                    Mail- <a href="mailto:contact@appsturf.com">contact@appsturf.com</a><br>
                    <p class="footerstyle">&copy; 2016 Appsturf Technologies Pvt Ltd </p>
                </div>
              </div>
        </div> 
    </section>
  </div>


  <footer class="">
    <div class="content">
      <div id="footerleft"> <span>BE SOCIAL WITH US</span><br>
        <ul class="social-icons">
            <li><a href="https://www.facebook.com/appsturf" target="_blank" ><img src="images/work/fb.png" class="homeicon hue-rotate"></a></li>
            <li><a href="https://plus.google.com/106803749715716637707" target="_blank" ><img src="images/work/gp.png" class="homeicon hue-rotate"></a></li>
            <li><a href="https://twitter.com/appsturf" target="_blank"><img src="images/work/tw.png" class="homeicon hue-rotate"></a></li>
        </ul>
      </div>
      <div id="footerright"> <span>CONTACT</span> <strong>509, Spaces 912, Mira Bhayandar Rd,
        Pleasant Park, Mira Road East,</br>
        Mumbai, Maharashtra 401107
        </strong><br>
        <a href="tel:+91 7709 805 786" class="homePhone"> +91 7709 805 786</a>,<a href="tel:+91 9665 006 351" class="homePhone">+91 9665 006 351</a>
        <br>
         Mail- <a href="mailto:contact@appsturf.com">contact@appsturf.com</a><br>
        
         <p class="footerstyle">&copy; 2016 Appsturf Technologies Pvt Ltd </p>
      </div>
    </div>
  </footer>
</div>

    <!-- menu baar scroller      -->

    <script type="text/javascript" src="script/interaction.js"></script>
    <script>
      (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
      (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
      m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
      })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

      ga('create', 'UA-67030621-1', 'auto');
      ga('send', 'pageview');

    </script>


</body>

  <script type="text/javascript">
if( 'ontouchstart' in window ){ var click = 'touchstart'; }
  else { var click = 'click'; }


  $('div.burger').on(click, function(){

      if( !$(this).hasClass('open') ){ openMenu(); } 
      else { closeMenu(); }

  });
    


  function openMenu(){
    
    $('div.circle').addClass('expand');
          
    $('div.burger').addClass('open'); 
    $('div.x, div.y, div.z').addClass('collapse');
    $('.menuburger li').addClass('animate');
    
    setTimeout(function(){ 
      $('div.y').hide(); 
      $('div.x').addClass('rotate30'); 
      $('div.z').addClass('rotate150'); 
    }, 70);
    setTimeout(function(){
      $('div.x').addClass('rotate45'); 
      $('div.z').addClass('rotate135');  
    }, 120);
    
    

  }
  
  function closeMenu(){

    $('div.burger').removeClass('open');  
    $('div.x').removeClass('rotate45').addClass('rotate30'); 
    $('div.z').removeClass('rotate135').addClass('rotate150');        
    $('div.circle').removeClass('expand');
    $('.menuburger li').removeClass('animate');
    
    setTimeout(function(){      
      $('div.x').removeClass('rotate30'); 
      $('div.z').removeClass('rotate150');      
    }, 50);
    setTimeout(function(){
      $('div.y').show(); 
      $('div.x, div.y, div.z').removeClass('collapse');
    }, 70);                         
    
  }
</script>
</html>
