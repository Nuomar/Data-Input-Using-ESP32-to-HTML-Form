
# Data Input Using ESP32 to HTML Form

2 types of HTML forms:

1.  The one that handles input data
2.  The one that also stores input data in SIPIFFS

Upload the sketch to the ESP32 after it has been successfully compiled, and then open the serial monitor to obtain the web server's IP address.

![enter image description here](https://i.postimg.cc/x1mdQ6RR/1-0b-TWErg5-LVcxg-TEBOIc-YLA.png)

We will see a view of the HTML form with three input fields after entering the IP address into the web server.

![enter image description here](https://i.postimg.cc/zfSXb34H/1-U8m-Gv-CQh-IDbf-Q2l697-FRRw.png)

Let’s try entering ‘55 in the input2 field.

![enter image description here](https://i.postimg.cc/Xv0YY910/1-Ns-Ut-Ivg831-Hh-Qq-Le-Hdx-OCw.png)

The page with the URL 192.168.1.9/get?input1=halo will then be redirected to. Quite intriguing, huh? If we go back to the main page, we may now enter various values in each field. This HTML form's initial effort is here.

Let's go to the second investigation.

# Saving Input Results to SPIFFS

Next, we upload the sketch and use the serial monitor to obtain the web server's IP address.

![enter image description here](https://i.postimg.cc/RV2Mg2tR/Tqw.png)

As seen above, the serial monitor also displays the results of input into the HTML form field in addition to the IP address. The values for all input variables named inputString, inputInt, and inputFloat are null or zero because we haven't entered any values—we haven't even opened the box yet.

Let's now launch a web browser and access the web server by entering the IP address from before.

![enter image description here](https://i.postimg.cc/DZXBFJZH/1-YDh-Hekp3-Aaaf-Dc-V2d0-Ggug.png)

So in here we input the values ​​’halo’, 18, and 3.3 to the three input fields. Input values ​​are adjusted to the type of data received by each input field, that’s right.
![enter image description here](https://i.postimg.cc/FHxjybdh/CyxcRJw.png)
