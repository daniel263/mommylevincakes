<template> 
<meta name="viewpoint" content="width=width-device-width, initial-scale=1.0">
<section>
<div class="circle"></div>
<div class="circle1"></div>
<div class="content">
  <div class="textbox">
    <h2>Just Name Your Flavour <br><span>We Cake IT</span>  </h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta quis nulla obcaecati magnam, voluptates ratione voluptatum esse? Omnis libero inventore commodi. Doloribus obcaecati dolorem provident aliquid corporis officia recusandae nulla.</p>
    <router-link :to="{name:'Cakegallery'}">View our Cakes </router-link>
  </div>
  <div class="imgbox">
    <img src="../assets/slice.jpeg" alt="Cake Slice" width="400" height="400" >
  </div>
</div>
</section>
</template>

<script>


export default {
}
</script>
<style scoped>
*{
  font-family:ubuntu;
}
section{
  margin-top: 5px;
  position:relative;
  width:100%;
  min-height: 100vh;
  padding:100px;
  display: flex;
  justify-content: space-between;
  align-items:center;
  background:#fff; 

}
.content{
  position: relative;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.content .textbox{
  position:relative;
  max-width: 800px;
}
.content .textbox h2{
  color: #1ca1f8;
  font-size: 2em;
  line-height: 1.3em;
  font-weight: 300;
}
.content .textbox h2 span{
  color:#f00e56;
  font-size: 1em;
  font-weight: 400;
  background: #fff;
  border-radius: 5px;
  
}
.content .textbox p
{
  color: #333;
  font-size: 1em;

}
.content .textbox a{
  display: inline-block;
  margin-top: 20px;
  padding: 8px 20px;
  background:#3d2827;
  color:#fff;
  border-radius:8px;
  text-decoration: none;
  letter-spacing: 1px;
}
.content .textbox a:hover{
  font-weight: bold;
  background-color: #f00e56;
  font-size: 1.1em;
  letter-spacing: 2px;
}
.content .imgbox{
  width:400px;
  display:flex;
  justify-content: flex-end;
  padding-right: 1px;
  
  

}
.content .imgbox img {
  
  border-radius:80px;
  max-width: 500px;

}
.circle{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(500px at right 800px)
}
.circle1{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(400px at left 100px)
}

</style>
