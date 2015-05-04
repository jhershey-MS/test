|Page Regions | Associated Files | More Information |
|-------------|------------------|------------------ |
| Ribbon | Any of the default master pagers. <br/>CorrespondingCSS <ul><li>Main Body – body: #s4-worspace</li><li>Suite bar – Left: #suiteBarLeft</li><li>Suite Bar – Right: @suiteBarRight</li><li>Ribbon container: #globalNavBox</li></ul> | Can be hidden via the Focus on Content button |


Filtering test

<script type="text/javascript">
        function filter()
        {
            alert("Filter selected");
            evaporate();
            disevaporate();
        }

        function evaporate()
        {
           
            if (document.getElementById("andCheck").checked == false)
                {
                var androids = document.getElementsByClassName("android");

                for (i = 0; i < androids.length; i++) {
                    androids[i].style.display = "none";
                }
            }
            if (document.getElementById("jsCheck").checked == false) {
                var javascripts = document.getElementsByClassName("js");
                for (i = 0; i < javascripts.length; i++) {
                    javascripts[i].style.display = "none";
                }
            }

           

            if (document.getElementById("winCheck").checked == false) {
                var wins = document.getElementsByClassName("windows");

                for (i = 0; i < wins.length; i++) {
                    wins[i].style.display = "none";
                }
            }

            if (document.getElementById("iosCheck").checked == false) {
                var apples = document.getElementsByClassName("ios");

                for (i = 0; i < apples.length; i++) {
                    apples[i].style.display = "none";
                }
            }

        }

        function disevaporate()
        {

            if (document.getElementById("andCheck").checked == true) {
                var androids = document.getElementsByClassName("android");

                for (i = 0; i < androids.length; i++) {
                    androids[i].style.display = "block";
                }
            }
            if (document.getElementById("jsCheck").checked == true) {
                var javascripts = document.getElementsByClassName("js");

                for (i = 0; i < javascripts.length; i++) {
                    javascripts[i].style.display = "block";
                }
            }

           

            if (document.getElementById("winCheck").checked == true) {
                var wins = document.getElementsByClassName("windows");

                for (i = 0; i < wins.length; i++) {
                    wins[i].style.display = "block";
                }
            }


            if (document.getElementById("iosCheck").checked == true) {
                var apples = document.getElementsByClassName("ios");

                for (i = 0; i < apples.length; i++) {
                    apples[i].style.display = "block";
                }
            }

        }
 </script>
    
  #This is the form for the filter

 <form>
 <input type="checkbox" id="andCheck" name="android" onchange="filter()" />Android
 <input type="checkbox" id="jsCheck" name="javascript" onchange="filter()" />JavaScript
 <input type="checkbox" id="iosCheck" name="ios" onchange="filter()" />iOS
 <input type="checkbox" id="winCheck" name="windows" onchange="filter()" />Windows
 </form>
  
##These are our test paragraphs

My common block of text 1

 <span class="android">
 My Android block of text 1
 </span>

 <span class="ios">
 My iOS block of text
 </span>

 <span class="windows">
 My Windows block of text 1
 </span>

 My common block of text 2
 
 <span class="android ios">
 My Andrioid and iOS block of text 1
 </span>

 <span class="android ios js">
 My Andrioid and iOS and Javascript block of text 1
 </span>

 <span class="js">
 My Javascript block of text 1
 </span>

 <span class="android">
 My Android block of text 2
 </span>

<span class="js">
My Javascript block of text 2
</span>
