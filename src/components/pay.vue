<template>
   <div class="cart-product-info">
        <a class="btn-buy fr" href="javascript:;">立即支付</a>
        <p class="fr product-total">￥<span></span></p>
        <p class="fl check-num"><span></span>张票总计：</p>
    </div>
</template>
<style>
        .page-shopping-cart .cart-product-info .btn-buy {
            height: 50px;
            color: #fff;
            font-size: 20px;
            display: block;
            width: 150px;
            background:#39e;
            text-align: center;
            margin-left: 30px;
        }
        .page-shopping-cart .cart-product-info {
            height: 50px;
            line-height: 50px;
            background: #f7f7f7;
            padding-left: 20px;
        }
        .page-shopping-cart .cart-product-info .product-total {
            font-size: 14px;
            color: #2654e9;
        }
        .page-shopping-cart .cart-product-info .product-total span {
            font-size: 20px;
        }
        .page-shopping-cart .cart-product-info .check-num {
            color: #333;
        }
        .page-shopping-cart .cart-product-info .check-num span {
            color: #2654e9;
        }
        .page-shopping-cart .cart-product-info .keep-shopping {
            color: #666;
            margin-left: 40px;
        }
        .page-shopping-cart .cart-product-info .keep-shopping span {
            display: inline-block;
            vertical-align: top;
            margin: 18px 8px 0 0;
            width: 15px;
            height: 15px;
        }
</style>

<script>
export default {
  
        
}
</script>


