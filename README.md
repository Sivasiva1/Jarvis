# Jarvis

Project : Iron Man Jarvis AI Desktop Voice Assistant 


Have you ever wondered how cool it would be to have your own A.I. assistant? Imagine how easier it would be to send emails without typing a single word, doing Wikipedia searches without opening web browsers, and performing many other daily tasks like playing music with the help of a single voice command. In this tutorial, I will teach you how you can make your personal A.I. assistant using Python. 

What can this A.I. assistant do for you?
It can send emails on your behalf.
It can play music for you.
It can do Wikipedia searches for you.
It is capable of opening websites like Google, Youtube, etc., in a web browser.
It is capable of opening your code editor or IDE with a single voice command.
Enough talks! Let's start building our own J.A.R.V.I.S.

Starting VS Code

              I am going to use the VS Code IDE in this video. Feel free to use any other IDE you are comfortable with. Start a new project and make a file called jarvis.py.

Defining Speak Function

              The first and foremost thing for an A.I. assistant is that it should be able to speak. To make our J.A.R.V.I.S. talk, we will make a function called speak(). This function will take audio as an argument, and then it will pronounce it.

Now, the next thing we need is audio. We must supply audio so that we can pronounce it using the speak() function we made. We are going to install a module called pyttsx3.

What is pyttsx3?
                  A python library that will help us to convert text to speech. In short, it is a text-to-speech library.
It works offline, and it is compatible with Python 2 as well as Python 3.

n case you receive such errors: 

No module named win32com.client
No module named win32
No module named win32api
Then, install pypiwin32 

What is sapi5?
    Microsoft developed speech API.
    Helps in synthesis and recognition of voice.
    What Is VoiceId?
    Voice id helps us to select different voices.
    voice[0].id = Male voice 
    voice[1].id = Female voice
Writing Our speak() Function :
                      We made a function called speak() at the starting of this tutorial. Now, we will write our speak() function to convert our text to speech

Creating Our main() function: 
                      We will create a main() function, and inside this main() Function, we will call our speak function.

Defining Wish me Function :
                      Now, we will make a wishme() function that will make our J.A.R.V.I.S. wish or greet the user according to the time of computer or pc. To provide current or live time to A.I., we need to import a module called datetime. 

Now, let's start defining the wishme() 

Defining Take command Function :
                                The next most important thing for our A.I. assistant is that it should take command with the help of the microphone of the user's system. So, now we will make a takeCommand() function.  With the help of the takeCommand() function, our A.I. assistant will return a string output by taking microphone input from the user.Before defining the takeCommand() function, we need to install a module called speechRecognition.

Coding logic of Jarvis

 Now, we will develop logic for different commands such as Wikipedia searches, playing music, etc.

Defining Task 1: To search something on Wikipedia 
                            To do Wikipedia searches, we need to install and import the Wikipedia module into our program. Type the below command to install the Wikipedia module 

Defining Task 2: To open YouTube site in a web-browser
                           To open any website, we need to import a module called webbrowser. It is an in-built module, and we do not need to install it with a pip statement; we can directly import it into our program by writing an import statement.

Defining Task 3: To open Google site in a web-browser
                          We are opening Google in a web-browser by applying the same logic that we used to open youtube. 

Defining Task 4: To play music 
                          To play music, we need to import a module called os. Import this module directly with an import statement.

Defining Task 5: To know the current time
                          we are using the datetime() function and storing the current or live system time into a variable called strTime. After storing the time in strTime, we are passing this variable as an argument in speak function. Now, the time string will be converted into speech

Defining Task 6: To open the VS Code Program
                           open the VS Code or any other application, we need the code path of the application.

Defining Task 7: To send Email
                            To send an email, we need to import a module called smtplib.

What is smtplib?

                                Simple Mail Transfer Protocol (SMTP) is a protocol that allows us to send emails and route emails between mail servers.                   An instance method called sendmail is present in the SMTP module. This instance method allows us to send an email.  It takes 3 parameters:
                                The sender: Email address of the sender.
                                The receiver:  Email of the receiver.
                                The message: A string message which needs to be sent to one or more than one recipient.
Defining Send email function :
                                We will create a sendEmail() function, which will help us send emails to one or more than one recipient.

Calling sendEmail() function inside the main() function:
                                We are using the try and except block to handle any possible error while sending emails.

Recapitulate:
                                First of all, we have created a wishme() function that gives the greeting functionality according to our A.I system time.
                                After wishme() function, we have created a takeCommand() function, which helps our A.I to take command from the user. 
                                This function is also responsible for returning the user's query in a string format.
We developed the code logic for opening different websites like google, youtube, and stack overflow and Leetcode.
                                Developed code logic for opening VS Code or any other application.
At last, we added functionality to send emails.

Is it an A.I.?
                                Many people will argue that the virtual assistant that we have created is not an A.I, but it is the output of a bunch of the statement. But, if we look at the fundamental level, the sole purpose of A.I develop machines that can perform human tasks with the same effectiveness or even more effectively than humans.

It is a fact that our virtual assistant is not a very good example of A.I., but it is an A.I.!

The E.N.D.
              With this, you have successfully made your very first virtual assistant. Explore and try to add other functionalities to J.A.R.V.I.S. I hope you all have liked this tutorial. Feel free to ask your queries in the QnA section.
