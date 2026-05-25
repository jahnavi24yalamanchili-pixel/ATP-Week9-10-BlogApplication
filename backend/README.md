### Project Description
---author(registration, login, add article, view articles, edit and del articles)
---user(registration, login, view articles, write comments)
---admin (login, view articles, block and activate user)


### BACKEND
1. generate package.json (npm init -y)
    change type to module, main to server.js
2. add dependencies for package.json
    - express (npm install express)
    - mongoose (npm install mongoose)
3. create .env for environment variables
    add db url : DB_URL= mongodb://localhost:27017/blogDB
    add port no : PORT = 7777
4. create http server
5. connect to db
    install dotenv : npm install dotenv
    import config function and call it
    to get values from .env file
        process.env.DB_URL
6. add middlewares
7. design schemas and create models
8. design apis for all resources
9. create services folder to define login and registration functions

--- tasks
function declaratipn vs fn expression

-----cookie concept:
when user logins for the first time , after login is successful token is stord in cookie
- next for any other request the token is present in cookie is verified
- for public routes token is not checked
- for protected routes token is checked 

------ fetch vs axios
FETCH
    - get request
        let resobj= await fetch (" ",method:"GET")
        //errors should be manually handled
        if (res.status!=200)
            throw new Error("")
        let res= await resobj.json() //message payload
    - post request:


AXIOS
    - error handling is handled
    - get request
        let resobj=await axios.get(" ")
        let res=resobj.data // message, payload
    - post request
        let res=await axios.post(" ",obj)



----- TO READ
- Toaster

