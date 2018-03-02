# southwest checkin
be the first to check in &amp; get those good seats :)

```javascript
        __|__
\________(_)________/
      O  ' '  O  
      
//enter flight time here Example: "7:30:00 PM"
var flightTime = "7:30:00 PM";

//get the checkin button
var checkIn = document.getElementById("submitButton");
//get ms for checkin time
var today = new Date();
var flightDate = (today.getMonth()+1) +'/'+ today.getDate() +'/'+ today.getFullYear();
var flightTimeMil = new Date( flightDate + ' ' + flightTime ).getTime();
//get current ms and find difference for timer
timeMil = new Date().getTime();
countDownMil = flightTimeMil - timeMil;
//set timer and click button function
function checkedIn () {
	checkIn.click();
	console.log ('Checked in first!');
};
setTimeout(checkedIn, countDownMil);
```

[open url](https://www.southwest.com/flight/retrieveCheckinDoc.html), enter flight info, and paste js in browser console.
