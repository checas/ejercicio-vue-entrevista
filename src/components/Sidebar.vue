<template>
    <div class="container">
        <div class="row">
            <div class="col-4">
                <h1 class="text-white pt-3 pb-5 text-center">
                    Macnally
                    <i class="bi-square" style="font-size: 3rem; color: white;"></i>    
                </h1>
                <ul class="pt-4">
                    <li v-for="a in menus1" :key="a.id" class="text-light pb-3">
                        <button type="button" class="btn btn-secondary">
                            <i :class= a.icon style="font-size: 1rem; color: white;"></i> {{a.menu}}
                        </button>
                    </li>
                    <p class="text-light pt-3 pb-3"> USA API</p>
                    <li v-for="a in menus2" :key="a.id" class="text-light pb-3">
                        <button type="button" class="btn btn-secondary">
                            <i :class= a.icon style="font-size: 1rem; color: white;"></i> {{a.menu}}
                        </button>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "PxAssetsTable",
    data(){
        return{
            menus1: [
                {
                    menu: 'Companies',
                    icon: 'bi-layout-sidebar'
                },
                {
                    menu: 'Investments News',
                    icon:'bi-calendar4-week',
                },
            ],
            menus2: [
                {
                    menu: 'Dashboards (Quandl)',
                    icon: 'bi-house',
                },
                {
                    menu: 'Top Markets News',
                    icon: 'bi-layout-sidebar'
                },
                {
                    menu: 'Stock details (iexcloud)',
                    icon: 'bi-shop-window',
                    
                },
                {
                    menu: 'Fundamentals India (Quandl)',
                    icon: 'bi-x-diamond',
                },
                {
                    menu: 'Robour global stock select (Quandl)',
                    icon: 'bi-x-diamond',
                },
            ],
        }
    },
}
</script>

<style scoped>
    .container{
        margin-left: 0;
        padding-left: 0;
    }
    .col-4 {
        height: 100vh;
        background-color: #293042;
    }
    li {
        list-style-type: none;
    }
    button {
        border: none;
        background: none;
        box-shadow: none;
    }
</style>

