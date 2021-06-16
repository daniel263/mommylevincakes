<template>
<main>
    <section class="gallery">
        <div class="cakes" v-for="cake in cakes " :key="cake.id">
            <div class="cake-inner">
                <div class="cake-text-wrap">
                    <h2 class="bg-text">{{cake.flavour}}</h2>
                </div>
            </div>
        <div class="cake-img-wrap">
            <img :src="cake.img" alt="flavour" class="image" height="300" width="300" >
        </div>
        <div class="cake-detail">
            <h2>{{cake.flavour}}</h2>
                <p>Prices: Small $30</p>
        </div>
    </div>
    </section>
     
</main>
 
</template>
<script>
export default {
    data(){
        return{
            cakes :[
                {
                    flavour: 'Chocolate',
                    img:require('../assets/choc.jpeg'),
                    id: 1 
                },
                {
                    flavour: 'Chocolate and Mint',
                    img:require('../assets/chocmint.jpeg'),
                    id: 2 
                },
                {
                    flavour: 'Chocolate, Mint and Vanilla',
                    img:require('../assets/chocminvan.jpeg'),
                    id: 3 
                },
                {
                    flavour: 'Chocolate and Vanilla',
                    img:require('../assets/chocval.jpeg'),
                    id: 4 
                },{
                    flavour: 'Chocolate',
                    img:require('../assets/choco.jpeg'),
                    id: 5
                },
                {
                    flavour: 'Lemon and Vanilla ',
                    img:require('../assets/lemonvan.jpeg'),
                    id: 6 
                },
                {
                    flavour: 'lemon',
                    img:require('../assets/lemon.jpeg'),
                    id: 7 
                },
                {
                    flavour: 'RedVelvet',
                    img:require('../assets/redvev.jpeg'),
                    id: 8 
                },
            ]
    }
}
}
</script>
<style scoped>
*{
    margin-left:0; 
    padding: 0;
    box-sizing: border-box;
    

}
body{
    font-family: 'montseratt', sans-serif;
}
main {
    width:100vw;
    min-height: 100vh;
    overflow: hidden;
    background-color:#eee ;
    display: flex;
    justify-content: center;
    align-items: center;
}
.gallery{
    display: grid;
    grid-template-columns: auto auto ;
    
    padding: 25px;
    margin:0 auto;
    border: 1px solid #ccc;
}
.cakes{
    width: 100%;
    padding:25px;
    }
.cake-inner{
    position: relative;
    padding: 5px;
    box-shadow: 0px 0px 16px rgba(0, 0, 0,0.25);
}


.cake-detail{
    padding:25px;
    margin: 0px -25px -25px;
   
}
</style>