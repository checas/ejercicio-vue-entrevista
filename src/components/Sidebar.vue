<template>
    <div class="container">
        <div class="row">
            <div class="col-4">
                <h1 class="text-white pt-3">Macnally</h1>
                <ul class="pt-4">
                    <li v-for="a in menus1" :key="a.id" class="text-light">
                        {{a.menu}}
                    </li>
                    <p class="text-light pt-3"> USA API</p>
                    <li v-for="a in menus2" :key="a.id" class="text-light">
                        {{a.menu}}
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
                {menu: 'Companies'},
                {menu: 'Investments News'}
            ],
            menus2: [
                {menu: 'Dashboards (Quandl)'},
                {menu: 'Top Markets News'},
                {menu: 'Stock details (iexcloud)'},
                {menu: 'Fundamentals India (Quandl)'},
                {menu: 'Robour global stock select (Quandl)'},
            ],
            items: [
                { mensaje: 'Foo' },
                { mensaje: 'Bar' }
            ]
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
    
</style>

