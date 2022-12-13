<template>
    <div class="products">
    <h1>Our Products</h1>
  </div>
<div class="container-fluid">
    <Div v-for="item in products" class="col-sm-3">
        <div class="card" style="width: 15rem;">
            <img :src="item.image" class="card-img-top picture" alt="productImage">
            <div class="card-body">
                <h3 class="card-title">{{item.name}}</h3>
                <p class="card-text">{{item.description}}</p>
                <label class="card-text">R{{item.price}}</label><br>
                <button class="btn">Add To Cart</button>
            </div>
        </div>
    </Div> 
</div>
</template>
<script>
export default{
    data(){
        return{

            products:[{
                name: "red pen",
                image: "https://i.postimg.cc/jd9fFpnL/redPen.jpg",
                description:"This is just a red pen mate",
                price: 20
            },
            {
                name :"black pen",
                image: "https://i.postimg.cc/gcx8Hcrf/blackPen.jpg",
                description:"This pen is black ",
                price: 40
            },
            {
                name:"blue pen",
                image:"https://i.postimg.cc/jjjLqv7G/BluePen.webp",
                description:"This pen is blue even Gift can afford it, gift it to your loved ones",
                price: 3
                
            }
        ]
    }
    }
}
</script>
<style>
.picture{
    width: 18rem;
}
.btn {
    color: gold;
    background-color: black;
}
</style>