Chapter 1: Working Environment Setup


In order to run the scripts you need to install few things on your computer. 

You need to Install : 

1) Python Programming Language

   Download From Here - https://www.python.org/downloads
   I will recommend to download python 3 as it is more reliable
   (Download Accordingy of your Operating System {windows, macOS})

2) PyCharm (To Execute Python Commands Easily)
  
   Download from here - https://www.jetbrains.com/pycharm/download/
   (Download Community Version)
---------------------------------------------------------------------------------------------------

Chapter 2: Getting Telegram Api
  
   Go To my.telegram.org and login your telegram there,
   Now on the next page
   Click on the first option "API Development"
   enter the required information
  (you may use random keywords but make sure you enter the same keywords in all three options)
   Now hit Enter
   You will see your Api id and Api hash
   copy them and save them in a notepad or in excel file along with Mobile Number
---------------------------------------------------------------------------------------------------

Chapter 3: Scrapping Members from a specific Group
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                               
                                 ""PART 1"" ((MANUAL INSTALLATION OF MODULES REQUIRED))---

                         (((( Open PyCharm
                              On TopLeft 
                              Click File >> Open 
                              Now Browse for the script folder
                              and select scrapper.py

                              Now again click on File >> Settings >> "Project: XXXXX"
                              Select Python Interpreter
                              There will be option written as 'Python Interpreter: <No interpreter>'
                              Change <no interpreter> to "Python 3.8" (as of your python version)
                              Now click on '+' sign on the right side
                              and search for "Telethon"
                              Select the package telethon and click 'install package' in the bottom
                              Also
                              Search for "Pyfiglet"
                              select the package 'pyfiglet' and install it from the install button at the bottom  ))))

                                                      """""""""""OR"""""""""""

                                 ""PART 2"" ((DIRECT INSTALL MODULES))---


                         (((( Open PyCharm
                              At the bottom You will see four OPTIONS
                              One of them will be Terminal
                              Open "Terminal"
                              type "pip install telethon"
                              it will automatically install telethon
                              when it is successfully installed
                              type "pip install pyfiglet"
                              it will install pyfiglet
                              
                                                    [[[USE ANY ONE PART EITHER PART ONE OR PART TWO]]]
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


   when install finishes
   go back to your code in PyCharm
   
   from 11th line
   enter your api id (change 0 to your api)
   enter your api hash (change 0 to api hash, it must be in inverted commas)
   enter your phone number

   move down to line 28
   now change XXXXXXXXX to the group username you want to scrape members
   in line 33
   Change XXXXXXX to your PC name
   
   Now Right Click Anywhere On The Screen
   And select "run 'scrapper'"

   It will ask for the OTP sent to your Telegram app
   enter OTP and hit enter

Done, Members successfully got SCRAPED as members.csv
---------------------------------------------------------------------------------------------------

Chapter 4: Removing Unwanted USERS

    Open Members.csv using Microsoft Excel
    now right click on 'username' or "B1" on the top
    Select 'filter' and choose "Filter by selected cells value"
    Now left click on the filter logo on the 'username' or "B1"
    scroll down and select [Blanks] and hit OK

    Now CTRL + A to select all empty users
    and click del to remove all empty users

    on the top left 
    there will be a logo to save the file
    click it and save it 

     OR
  
   press CTRL + S to save
---------------------------------------------------------------------------------------------------

Chapter 5: Adding Members to group

    Open PyCharm
    On TopLeft 
    Click File >> Open 
    Now Browse for the script folder
    and select groupadder.py
    
    again enter api id, api hash and phone number
    in line 25, 'change XXXXXX to your PC name' or 'Browse to members.csv'

    Now run the script
    it will ask for otp sent to your telegram app
    enter otp
    hit enter
    
    It will Show you group list along with a specific number
    and it will ask you to enter a number
    enter your group (the group you want to add members to) number
    hit enter
    
    it will ask you StartFrom 
    Enter 1
    It will ask you EndTo
    Enter 50
    hit enter

    It will start adding members to your group

  
    ""You can add only 50 members per account in 6 hours
    so be ready with as many telegram accounts as you want""

   With another account,
   start from 50 and end to 100 and so on
---------------------------------------------------------------------------------------------------

Chapter 6: Add to Channel
   
   open channeladder.py in PyCharm
   enter api id, api hash, and phone number
   in the next line (17th line) 
   enter your channel username inside the inverted commas
   for example
   channel_usename = 'MyChannelXYZ' (don't write @)
   now in line 26 enter the members.csv location

   now run the script
   it will ask you otp
   write otp and hit enter
   It will ask you Start From
   Enter 1
   It will ask you EndTo
   Enter 50
   hit enter

   It will start adding members to your channel

    ""You can add only 50 members per account in 6 hours
    so be ready with as many telegram accounts as you want""

   With another account,
   start from 50 and end to 100 and so on
---------------------------------------------------------------------------------------------------

Chapter 7: Sending Bulk Messages

   open smsbot.py in PyCharm
   enter api id, api hash and phone number
   now in line 26, enter members.csv location

   run the script
   enter otp
   enter StartFrom  (type 1)
   enter EndTo   (type 50)
   it will now ask you to write the message

   enter your message which yoy want to send members
   hit enter
 
   It will start sending messages to your targets

   With another account,
   start from 50 and end to 100 and so on
---------------------------------------------------------------------------------------------------

    
    