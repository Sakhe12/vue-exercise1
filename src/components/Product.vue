<template>
    <div class="container-fluid">
        <div class="row">
            <Div v-for="item in products" :key="item" class="col-sm-3 gap-3">
                <div class="card" style="width: 18rem;">
                    <img :src="item.imgSrc" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">{{item.name}}</h5>
                      <p class="card-text">{{item.surname}}</p>
                      <a href="#" class="btn btn-primary v-on:click">Add to checkout</a>
                    </div>
                  </div>
               </Div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Products',
    data(){
         return{
products: [
    {
        id: 1,
        name: "Thando",
        surname: "Beko",
        imgSrc : "https://picsum.photos/id/237/200/300"
    },
    {
        id: 2,
        name: "Gift",
        surname: "Mahlangu",
        imgSrc : "https://picsum.photos/200/300"
    },
    {
        id: 3,
        name: "Sakhe",
        surname: "Mzolisa",
        imgSrc : "https://picsum.photos/200/300"
    },
    {
        id: 4,
        name: "Jeff",
        surname: "Ricardo",
        imgSrc : "https://picsum.photos/id/237/200/300"
    }
]
        }
    }

}
</script>
<style lang="">
    
</style>