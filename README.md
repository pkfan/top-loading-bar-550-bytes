# top-loading-bar-550-bytes
# TOP PRELOADING BAR with html css javascript

This is amazing flexible HTML CSS Javascript 20 lines CODES TOP LOADING BAR with different colors. 

you can change colors and loading times according to your needs. 

Top loading bar will disapear after page fully loaded to browser windows.

Default time is 2 second, but if page is loaded before 2 second, top load bar will diappear.

Minimum compress size of this code is 550 bytes, so you can add HTML5 CSS3 JAVASCRIP top preloading bar without any performance issue of page.




![alt text](https://github.com/pkfan/top-loading-bar-550-bytes/blob/main/top-load-bar%20(1).gif)



![alt text](https://github.com/pkfan/top-loading-bar-550-bytes/blob/main/top-load-bar%20(2).gif)



![alt text](https://github.com/pkfan/top-loading-bar-550-bytes/blob/main/top-load-bar%20(3).gif)




# paste this code after start (body element)
```
<!-- paste this code after <body> start element -->
<!-- start preloader -->
<section id="topbar-preloader">
    <style>
        #preloader{
            /* change color of preloader bar according to your needs */
            /* background-image:linear-gradient(to right,#9CECFB,#65C7F7,#0052D4); */
            background-image:linear-gradient(to right,#cc2b5e,#753a88);

            height: 3px;
            z-index: 1000; 
            position: fixed; 
            top: 0;        
        }
    </style>
    <div id="preloader">
    </div>
    <!-- preload script -->
    <script>
        let preloaderBar = document.querySelector('#preloader');
        let idForIntervalCleaning = setInterval(incrementWidth, 20); //  20*100=2000 mili second or 2 second
        let width = 0;

        // increment function
        function incrementWidth(){
            if (width >= 90) {
                clearInterval(idForIntervalCleaning);
            } 
    else {
                width++; 
                preloaderBar.style.width = width+"%";
            }
        }

        window.addEventListener('load', () => {
            
                preloaderBar.style.display = "none";
                clearInterval(idForIntervalCleaning);
        });
    </script>
</section>
<!-- end preloader -->
```

  
  

# compress verson of preloading top bar code
```
<section id="topbar-preloader">
<style>#preloader{background-image:linear-gradient(to right,#cc2b5e,#753a88);height:3px;z-index:1000;position:fixed;top:0}</style>
<div id="preloader">
</div>
<script>let preloaderBar=document.querySelector('#preloader');let idForIntervalCleaning=setInterval(incrementWidth,20);let width=0;function incrementWidth(){if(width>=90){clearInterval(idForIntervalCleaning);}
else{width++;preloaderBar.style.width=width+"%";}}
window.addEventListener('load',()=>{preloaderBar.style.display="none";clearInterval(idForIntervalCleaning);});</script>
</section>
```
