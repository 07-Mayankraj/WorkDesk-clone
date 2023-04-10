
![logo](https://user-images.githubusercontent.com/87657007/221491845-03166e0e-baa5-4077-957c-7924e578afa1.png)
# WorkDesk https://workdesk.netlify.app/

Reatime screen sharing web application..



## Tech Stack

**Client:** HTML,CSS, Javascript,Bootsrap

**Server:** Node.js, Express.js , MongoDB, WebRTC, PeerJS library, Socket.io


## Frontend Part

- Home page
- Login/Signup

## Backend Part
- Authentication using JWT
- Mongoose - connecting the database
- Server side -->> Node.js and Express 
### Database - 
    - MongoDB

## Features 
 -  Screen Sharing 
 -  Chatting 
 -  Video calling
## Application Guide



### To use {Screen share} feature -->
-  First Create room 
-  User can share the screen
-  Than user can join the room using room ID
-  Enter room ID to join 

#### Stop share -->
- Click on stop share option 

### To use {Video calling} feature -->
-  First Create room 
-  User can join the call by using the room ID
-  To end the call click on hang on button

### To use {Chat} feature -->
-  Enter the user name 
-  User can chat with online users
-  For online users  it will show green tick




## Examples
 #### Creating connection and accessing user media .
```javascript
    peer = new Peer(room_id);
    peer.on('open', (id) => {
        console.log("Peer has joined ID no", id);
        hideModal()
        // media options...
        getUserMedia({ video: true, audio: true },
            (stream) => {
                local_stream = stream;
                setLocalStream(local_stream)
            }, (err) => {
                console.log(err);
            })
        notify("Waiting for the member to join.")
    })
```

# Backend api endpoints
create user -> post: localhost:8080/user/register  
    sample data : 
    
    {
      "name": "User",
      "email": "User@gmail.com",
      "password": "User"
    }
  ---    

   - login user ->    post : localhost:8080/user/login 
   - get new token -> get  : localhost:8080/newtoken
   - logout user   -> get  : localhost:8080/logout
   - get all user   -> get  : localhost:8080/user 
   - get one user   -> get  : localhost:8080/user/id 

      while making get request from fontend
      we need to send access_key(presented in .env)



----------------------------------------------------------------

github Oauth 

    1. Route login,dashboard 
    2. impelement auth 
    3. sessions
    4. protected
    5. logout 

### Installation
To install the WorkDesk, follow these steps:

1. Clone the repository:
```
https://github.com/deepakChourasiya-aj/melted-group-7444.git
```

2. Install the dependencies:
```
cd melted-group
npm install
```

Start the server:
```
npm run server
```

You are good to go


<br>

System_design


![Untitled Diagram](https://user-images.githubusercontent.com/87657007/225451422-8d5c05ca-5046-4c10-b890-1f02bbcd3d73.jpg)

![image](https://user-images.githubusercontent.com/87657007/230957371-70c47d1a-fe86-4431-ba83-6f73acc68c42.png)
![image](https://user-images.githubusercontent.com/87657007/230957688-bc009463-c988-4e93-b035-a0f172504957.png)
![image](https://user-images.githubusercontent.com/87657007/230957711-afb14b7e-5039-480d-a1bb-e766ef23d07c.png)
![image](https://user-images.githubusercontent.com/87657007/230957726-4e853b3c-7799-4703-b327-f75e20bc092c.png)
![Screenshot (520)](https://user-images.githubusercontent.com/87657007/221489051-e6a06137-e7a4-42a7-9e5f-000eb14d6358.png)
![Screenshot (522)](https://user-images.githubusercontent.com/87657007/221489062-46235239-d888-4ca6-89fe-d5a8e4e05a48.png)
