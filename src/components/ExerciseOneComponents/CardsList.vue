<template>
    <div class="card-list  wrapper">
        <div class="spacer xxx-large"></div>
        <div class="card-list-container">
            <div class="card">
                <div class="card-content">
                    <img src="https://via.placeholder.com/400x300" alt="">
                    <div class="spacer small"></div>
                    <div class="card-desc">
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum gravida interdum. Quisque nec leo dapibus, luctus lorem a, sagittis augue. Cras volutpat magna eu odio fringilla, eu dictum lacus fringilla. 
                    </p> 
                
                    </div>
                    <button>Read More</button>
                </div>
            </div>
            <div class="card">
                <div class="card-content">
                    <img src="https://via.placeholder.com/400x300" alt="">
                    <div class="spacer small"></div>
                    <div class="card-desc">
                    <p> 
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum gravida interdum. Quisque nec leo dapibus, luctus lorem a, sagittis augue.
                    </p>
                    </div>
                    <button>Read More</button>
                </div>
            </div>
            <div class="card">
                <div class="card-content">
                    <img src="https://via.placeholder.com/400x300" alt="">
                    <div class="spacer small"></div>
                    <div class="card-desc">
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. In bibendum gravida interdum. Quisque nec leo dapibus, luctus lorem a, sagittis augue. Cras volutpat magna eu odio fringilla,
                        </p>                
                    </div>
                    <button>Read More</button>
                </div>
            </div>
        </div>
        <div class="spacer xxx-large"></div>
    </div>
</template>

<script>
export default {
     name: 'CardsList',
}
</script>

<style scoped>
.card {
    padding-left: 15px;
    padding-right: 15px;
    width: 30%;
    flex: 0 0 auto;  
}
.card-content {
    border: 1px solid #ddd;
    padding: 24px;
    border-radius: 5px;
    display: flex;
    flex-direction: column;
    align-items: center;
    box-shadow: 1px 1px 5px 4px rgba(0,0,0,0.05);
    -webkit-box-shadow: 1px 1px 5px 4px rgba(0,0,0,0.05);
    -moz-box-shadow: 1px 1px 5px 4px rgba(0,0,0,0.05);
    margin-bottom: 1rem
}
.card-list-container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap
}

img {
   width: 100%;
   height: 300px;
   object-fit: cover;
}
.card-desc {
    min-height: 300px;
}
.card-desc p{
    text-align: center;
    line-height: 1.3;
    font-size: 21px;
  
}

.card button {
    border: 3px solid #000;
    padding: 10px 20px;
    text-transform: uppercase;
    cursor: pointer;
    background: none;
    border-radius: 16px;
    font-weight: bold;
}

@media screen and (min-width: 640px) and (max-width: 1023px) {
    .card {
        width: 45%; 
        padding: 10px;
    }

    .card-desc {
        min-height: 400px;
    }
    
}

@media screen and (max-width: 639px) {
    .card {
        width: 100%; 
        padding: 0;
    }

    .card-desc {
        min-height: 370px;
    }
    
}



</style>