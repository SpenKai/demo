<template>
    <div class="page-shopping-cart" id="shopping-cart">
          <div class="cart-product-title clearfix">
              选择票种
            </div>
    <selectpicket></selectpicket>
    <info></info>
    <pay></pay>
    </div>
</template>

<style>
        .page-shopping-cart {
            width: 400px;
            margin: 50px auto;
            font-size: 14px;
            border: 1px solid #e3e3e3;
            border-top: 2px solid #317ee7;
        }
        .page-shopping-cart .cart-title {
            color: #317ee7;
            font-size: 16px;
            text-align: left;
            padding-left: 20px;
            line-height: 68px;
        }
        .page-shopping-cart .check-span {
            display: block;
            width: 24px;
            height: 20px;
        }
        .page-shopping-cart .td-num, .page-shopping-cart .td-price, .page-shopping-cart .td-total {
            width: 160px;
        }

        .page-shopping-cart .td-do {
            width: 150px;
        }
        .page-shopping-cart .cart-product-title {
            text-align: left;
            height: 38px;
            line-height: 38px;
            padding: 0 20px;
            background: #f7f7f7;
            border-top: 1px solid #e3e3e3;
            border-bottom: 1px solid #e3e3e3;
        }
        .page-shopping-cart .cart-product-title .td-product {
            text-align: center;
            font-size: 14px;
        }
        .page-shopping-cart .cart-product {
            padding: 0 20px;
            text-align: center;
        }
</style>

<script>
import selectpicket from './selectpicket.vue'
import pay from './pay.vue'
import info from './info.vue'
export default {
    components: {
        selectpicket,
        pay,
        info
    },
   
}
</script>