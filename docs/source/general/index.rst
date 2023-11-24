**********************
General Best Practices
**********************

.. toctree::
   :maxdepth: 2

   self

There are some generic general truths regardless of what language chosen for development. This is where those things shall be discussed in depth. 

Before you begin development
############################

Here are some things you should ask yourself and consider before you begin writing any code for any new project. And be completely honest with yourself. Don't just convince yourself this is needed just because you thought of it. 

1. Is there already a tool out there that does what I am trying to do?
  
  - If the answer is Yes
 
    1. Am I wanting to reinvent the wheel and build the exact same thing?
    2. Do I want to build something slightly different than what already exist?
    3. Do I want to fork the existing tool and add to it?  
  
  - If the answer is No
  
    1. Is there a userbase for such a tool? 
    2. Is the return really worth the investment to develop this tool?
    3. Does this tool provide value to the community? If so, what is that value?
   
2. Have I developed a roadmap of the code I want to write?
3. Have I developed a detailed list of functionality/features I want to provide in my tool?



What Type of Application?
#########################

Next to consider is what type of application you want to build. The 4 choices here are

1. Client Side
2. Server Side
3. Both Client and Server Side
4. A library to be used by other developers to do something

In case you are not sure what the difference between client side and server side are, it can really be summed up in 2 sentences. 

- A client side application is an application designed to run on the end users computer
- A server side application is designed to be hosted on a server somewhere and the end user access the application through other means

So, what are some examples of a client side application. Well a contact logger such as N3FJP, Log4OM, HAMRS. Winlink, WSJT-X, JS8Call are also client side applications. Now you are probably looking for some examples of server side applications. Sure those are out there too. Brandmeister for DMR talkgroups, APRS.fi, QRZ.com are all server side applications. Notice the difference here is if the end user has to install anything on their local machine to use the application or not. If they do, that is a client side application. If they don't, then it is a server side application. 

So, what is an example of where you would want to create both a server side and a client side application. A classic example of this is you developed an API based application to run in a hosting service that connects to a database to store data. You have various API endpoints to do this like retrieve data from the database, add data to the database, or manipulate existing data in the database. However, there is no web based front end to interact with this API. Instead you develop a client side application the end user installs on their local machine that then authenticates and interacts with the server side API you have developed. 

What about a library. Many languages support importing of packages/libraries. These are smaller bits of code that can be imported into your project and then used so you don't have to write the code to do it yourself. So let's say you ar working on writing a python application and you want to work with a JSON file for data management. you can then add `import json` to the top of your python application to import the `json` package and then use it to work with the JSON files instead of figuring out how to do that yourself. 