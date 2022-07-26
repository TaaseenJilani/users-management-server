# Node-Database

## What is it?

This is a node.js backend server where you can add, delete, access, and update users' information such as their first name, last name, and age. In order to make sure that each user is different, a unique id is used for each of them. 

## How to use

First, if you don't already have it downloaded, download node.js for your operating system from `nodejs.org`. Then you can download the files and open in on a text editor. 
In the terminal of the text editor, type `npm install --save express` to install express. In order to install nodemon, type `npm install --save-dev nodemon`. There are 4 
types of requests you can do with this server: get (access/ view user's data), post (create new user data), patch (update existing user data), and delete (delete user data). 
The only one of those requests that can be done from your browser is the get request, the other three requests are not possible with the browser. In order to be able to do 
the other three requests, you need to download postman (an API platform for developers) from `postman.com/downloads` for your appropriate operating system. Finally, to start 
the server, type `npm start` onto the terminal of the text editor you opened the files on. The port is set to 5000 by default, so that's the port that will open up on the browser. 
You should see `Hello from homepage` on the screen. Now, on the url bar, add `/users` at the end of `http://localhost:5000`. Now, in `http://localhost:5000/users`, you should see an
empty array (`[]`). Now, go onto postman and create the `+` symbol to crate a new request. 

To do a `POST ` request:

Choose `POST` from the dropdown menu. In the url bar, type in `http://localhost:5000/users`. Click on the `body` tab, and make sure that the text style (right most tab) is selected to 
JSON. In the body tab, type in the following: `{ "firstName": "John", "lastName": "Doe", "age": 25 }`. Then, click on the big `SEND` button on the right hand side of the url bar. 
If you now refresh your browser (making sure that you are at `http://localhost:5000/users`), you will see that person's details on the screen in the JSON format. You have now successfully added
a new user named John Doe who is 25 years old to the database. 
![image](https://user-images.githubusercontent.com/45811245/180939437-e2dedfd4-5e86-418b-a771-827af18ee14e.png)


To do a `GET` request:

Select `GET` from the dropdown menu, and click `SEND`. You should now be able to see all the users that you have added so far. 
![image](https://user-images.githubusercontent.com/45811245/180939487-99c05acb-3213-4ec0-8a29-724117b68438.png)


To do a `DELETE` request: 

Select `DELETE` from the dropdown menu, and click `SEND`. You should now be able to see through a get request that the user is deleted.
![image](https://user-images.githubusercontent.com/45811245/180939316-ce0fd4ad-6761-4598-984e-2125120b9ef5.png)


To do a `PATCH` request: 

Select `PATCH` from the dropdown menu, update the information about the user you want to update, and click `SEND`. You should now be able to see through a get request that the user has been updated according to your request.
![image](https://user-images.githubusercontent.com/45811245/180939221-395a1bf5-ddf5-43e1-9da1-6b2a171c95d3.png)
