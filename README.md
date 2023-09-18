# day-14-Home
First of all we will take a heading of project afrer that , we take a div that's class is clock and after that we a another div(child div)
  <div class="clock">
      <div>
        <span id="hour">00</span>
        <span class="text">Hours</span>
      </div>
  <div>
  Same task for minutes and second after that we apply  basic css and set the background image  of the our project.
<------------------------------------------------------------------------------------------------------------------------------------>
In the Java Script part we get the element by document.getElementById("") method ie-
  const hourEl = document.getElementById("hour");
  const minuteEl = document.getElementById("minutes");
  const secondEl = document.getElementById("seconds");
  const ampmEl = document.getElementById("ampm");

After that we create a function ( function updateClock() ) these function get update value of clock 
   let h = new Date().getHours();
   let m = new Date().getMinutes();
   let s = new Date().getSeconds();
   let ampm = "AM";
   
After that we chect the condition of AM and PM and after that we  conver the data (ie- minutes to hours)
   after that
     h = h < 10 ? "0" + h : h;
     m = m < 10 ? "0" + m : m;
     s = s < 10 ? "0" + s : s;
after we apply set time out function 
    setTimeout(() => {
    updateClock();
    }, 1000);
and  cell the function -: updateClock();
