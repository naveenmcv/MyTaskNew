# REACT

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
- 

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
    

