# connecting-the-web-page-to-the-serial-port
# set up:
1- Download the (speech recognition) zip file

1- Unzip the (speech recognition) zip file.

2- Open the speech recognition in an editor eg., Visual Studio.

3- Open the cmd or in the terminal section type "pip install flask" then click enter.

5- Run the (app.py) file.

6- Open the browser and type "http://127.0.0.1:5000" then click enter and you will web page is ready to use.

7- For speech recognition click the (start) button. For serial port connection click the (connect to the serial port) button.  

# Methodology:
# I.Connecting the web page to serial port:
   
    1- We need the Web Serial API which provides a way for websites to read from and write to a serial device using JavaScript.
    
    2- For connecting the web page to the serial port all you need is to make an input type button in a web page and copy these lines in JavaScript.
    
    document.querySelector('input').addEventListener('click', async () => {
    
    // Prompt user to select any serial port.
    
  const port = await navigator.serial.requestPort();
 
});
    
    3- For more details you can visit this useful website that I had the code from "https://bit.ly/3ABN241"

# II.Connecting the back-end with the front-end:
The speech-to-text recognition was done in python. Python is a back-end programing language. Unlike the language of the web page which is HTML. HTML is a front-end programing language. In order to connect the back-end with the front-end we to use a platform either Django or flask. In this project, the flask platform is used.
