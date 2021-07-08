# THREE_JS (Deploy))


##  $ {*** Index.html *** \over RUN}$




### indexe.html file
  ```js
  // ! boiler plate
  <body>
    src = "./three.js"
    src = "./Main.js"
  </body>
  
  ```

### >Three.js<

###  ** Main.js **



#### animate ( ++time++ renderer (scene, camera));
- 
  ```js
  var animate = function () {
    requestAnimationFrame( animate );
    cube.rotation.x += 0.1;
    renderer.render(scene, camera);  };
  animate();
  ```

#### renderer "still" ( scene, camera)
##### Scene ( "scene.add(cube)" ) 
###### cube ( ".mesh( geometry , material)" )

####### Object = geometry + material
- Geometry
- Material

##### camera

#### <<< pass the render stuff to body { document.body.appendChild( renderer.domElement); }



