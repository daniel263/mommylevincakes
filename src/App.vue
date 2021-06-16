<template>
<meta name="viewpoint" content="width=width-device-width, initial-scale=1.0">

  <div id="nav">
   <span> Mommy_Levin Cakes   |    </span> 
    <router-link :to="{name: 'Home'}">Home</router-link> |
    <router-link :to="{name: 'About'}">About</router-link> |
    <router-link :to ="{name:'Cakegallery'}">Cake Gallery</router-link>
  </div>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #111;
}

#nav {
  padding: 5px;
  text-decoration: none;
  justify-content: space-between;
  text-align: end;
  letter-spacing: 1px;
  font-family: 'comic neue';

}

#nav a {
  font-weight: normal;
  font-size: 1.2em;
  color: #3d2827;
  text-decoration: none;
  
}
#nav a:hover{
  font-weight: bold;
  color: #f00e56
}


#nav a.router-link-exact-active {
  color: #f00e56;
}
#nav span{
  color:#f00e56;
  font-weight: bold;
  font-family: Pacifico;
  font-size: 1.2em;
  }
@media(max-width:991px){
  section{
      padding: 20px;
  }
  .content{
    flex-direction: column;
    padding:10px;
    margin-bottom: 15px;
  }
  .content .textbox{
    margin-bottom: 25px;
    max-width: 100%;
  }
  .content .imgbox{
    max-width: 100%;
  }
  .content .imgbox img{
    max-width:250px;
  }
  .circle1{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(100px at left 100px)
}

}
</style>
