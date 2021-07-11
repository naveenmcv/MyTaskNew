# REACT

### REACT VSCODE COMMANDS
- clone the project into local folder
- run> npm install ( it will download the dependencies and store in 'node modules' folder) 
- npm start ( it will run the app in browser. we need to do this, since its an react app. otherwise we could have simple right click and do live server)
- npm build ( to optimise and export to production version)
- npm install -g serve
#### serve -s (if not working)
- -> > set-ExecutionPolicy RemoteSigned -Scope CurrentUser 
- -> > Get-ExecutionPolicy
- -> > Get-ExecutionPolicy -list

#### STOP = CTRL + C
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX




### how to run HTML build files >> to RUN locally
#### Git repo : drichard /mindmaps
- 
    ```js
    //https://github.com/drichard/mindmaps
    .- this is HTML5 project 
    This was way before React, ES6, webpack. Heck, it doesn't even use Backbone.
    However, there is no reason to change any of that and it makes the code     base quite easy to grok. 
    There is no compilation step, no babel plugins, no frameworks. Just a   JavaScript application and a very simple Model-View-Presenter pattern.
    ```

- 
    ```js
    - HTML5 stuff which was cool in 2011
    - 100% offline capable via ApplicationCache
    - Stores mind maps in LocalStorage
    - FileReader API reads stored mind maps from the hard drive
    - Canvas API draws the mind map
    ```

- 
    ```js

    //Build
    First run npm install to install required dependencies
    Run npm run start to launch a local dev server. The app will be hosted at   http://localhost:3000.
    Run npm run build to compile the production bundle. The artifacts will be   located in /dist.

    // Host yourself
    All you need is a web server for static files. After building, copy all     files from /dist into your web directory and launch the app with index. html. Make sure your web server serves .appcache files with the mime type    text/cache-manifest for the application to be accessible offline.

    In Apache add the following line to your .htaccess:

    AddType text/cache-manifest .appcache
    In nginx add this to conf/mime.types:

    text/cache-manifest appcache; 
    Alternatively, you can launch a local debug server with npm start which     starts a server on localhost:8080.
    ```
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

### how to run HTML build files >> to RUN locally SOLUTION
#### Git repo : drichard /mindmaps
- https://cli.vuejs.org/guide/deployment.html#general-guidelines
- 
    ```js
    //s

    Deployment
    #General Guidelines
    If you are using Vue CLI along with a backend framework     that handles static assets as part of its deployment,   all you need to do is make sure Vue CLI generates the     built files in the correct location, and then follow the    deployment instruction of your backend framework.

    If you are developing your frontend app separately from     your backend - i.e. your backend exposes an API for your    frontend to talk to, then your frontend is essentially a   purely static app. You can deploy the built content in    the dist directory to any static file server, but make     sure to set the correct publicPath.

    #Previewing Locally
    The dist directory is meant to be served by an HTTP     server (unless you've configured publicPath to be a     relative value), so it will not work if you open dist/  index.html directly over file:// protocol. The easiest    way to preview your production build locally is using a    Node.js static file server, for example serve:

    npm install -g serve
    # -s flag means serve it in Single-Page Application mode
    # which deals with the routing problem below
    serve -s dist
    #Routing with history.pushState
    If you are using Vue Router in history mode, a simple   static file server will fail. For example, if you used    Vue Router with a route for /todos/42, the dev server  has been configured to respond to localhost:3000/todos/  42 properly, but a simple static server serving a     production build will respond with a 404 instead.

    To fix that, you will need to configure your production     server to fallback to index.html for any requests that  do not match a static file. The Vue Router docs provides     configuration instructions for common server setups

    ```


XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

### 2


    ```
##### SRC important

###### 1. App.js ( HOLDS = LOGIN + HTML + CSS) in one file

-     
    ```js
    import React  from 'react' ; 3.4K ?

    // create a component by writing a function ( or class)

    // create function()

    function App(){
        return (
            <div>
                <h1> Hello React NNN </h1>
            </div>
        )

    }

    export default App; // exports his file to Index.js file ( which has the ReactDOM.renderer & root)

   ```


###### 2. index.js ( IT MOUNTS THE RECT APP)
- 
    ```js

    // come here after reading App.js

    import App from '.App';

    ReactDOM.render( <App/>, document.getElementByID('root'));
    // it renderes the APP in index.html ( in public folder)


   ```
    
###### 3. index.html
- 
    ```js
    <body>
    <div id='root'> // it gets all data from other files and renders here

    // if you check the web display 
    //you will see " Hello React NNN "
   ```

###### App.css ( some styling)
- 
    ```js
    .App-logo{
    animation :
    height :
    pointer-events:none;}

    .App-header{
    background-colour
    min-height:
    display:
    flex-direction
    align-items
    justifu-contect
    font-size
    color:
    }
   ```
     
   
###### App.test.js ( TEST - doesnt matter for this one)

###### index.css

- 
    ```js
     body{
      margin, padding, font-family
      -webkit-font-smoothing:
      -moz-osx-font-smoothing;
      }
      code{
      font-family:
      }


   ```
###### logo.svg
###### serviceWorker.js

###### 


XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX


### Steps
- install nodejs ( to use npm package manager)
- open any empty folder
- got to termincal and write 'npx create-react-app' >> creates the templates
- create scripts and use 'npm start' to preview
- //after completion
- create git repo
- //cmd code
- git remote add origin
- git remote set-url
- npm run build
- npm run deploy
- // install gh-pages if required
- npm run deploy
- // to should say PUBLISHED
- >npm install -g serve
.  -s flag means serve it in Single-Page Application mode
.  (#) which deals with the routing problem below
serve -s dist


XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
### INFO
##### Node modules ( all packages locally added - no need to touch)
- babel , reactDom

##### Public ( doesnt matter now)
###### favicon.ico
###### 3. index.html
- 
    ```js
    <body>
    <div id='root'> // it gets all data from other files and renders here

    // if you check the web display 
    //you will see " Hello React NNN "

    ```
###### manifest.json
- 
##### SRC
###### gitignore
- (has data information to exlude while uploading to git)



###### package-lock json
-
    ```js
    version of all each packages
    " @babel/helper-plugin "
    " version " : "7.4.3"

    }

###### package.json 

-
    ```js
    {"name" : "projectreact"
    "version" : "0.1.0"
    "private" : true,
    "dependencies":{ x,y, x}
    "scripts":{ x,y, x} start, build, test etc
    "eslintconfit":{ x,y, x}
    "browerlist":[ x,y, x]
    }
    
XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
### EXAMPLES
##### clientside applications
- 
    ```js
     I've always been developing my clientside applications 
     without any of my own servers running behind it, 
     using Webstorm's built-in webserver to serve my content.
    ```
-
    ```js
    other people use Node with Express to act as their webserver

    ```


-
    ```js
    //question
    Today most websites are not static documents anymore but are 
    files that get altered by javascript by manipulating the 
    DOM, so I don't think any html files should be considered as static files?
    
    //answer 
    The files for your pages themselves are still static. That is, you are not creating them dynamically with server-side code. What happens in the browser doesn't matter in this context... the idea is that you do not need to generate these files on the fly, as their content does not change.

    ```

-
    ```js
    dist/ The /dist stands for distributable. 
    The /dist folder contains the minimized version of the source code. 
    The code present in the /dist folder is actually the code 
    which is used on production web applications.
    

    ```

-
    ```js
    What is an AppCache file?
    An APPCACHE file is a file used by web browsers to enable 
    accessibility of  web applications when there is no network connection.
    

    ```

-
    ```js
    

    ```