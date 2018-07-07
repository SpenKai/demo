<template>
    <div class="cart-product clearfix">
        <table>
            <tbody>
            <!--遍历的时候带上索引-->
            <tr v-for="(item,index) in productList">
                
                <td class="td-product">
                    <div class="product-info">
                        <h3>{{item.pro_name}}</h3>
                        <p>{{item.pro_purity}}</p>
                    </div>
                    <div class="clearfix"></div>
                </td>
                <td class="td-price">
                    <p class="red-text"><span class="price-text">{{item.pro_price.toFixed(2)}}</span>元</p>
                </td>
                <td class="td-check">
                    <input type="radio" name="sel" @click="item.select=!item.select" :class="{'check-true':item.select}">
                </td>
            </tr>
            </tbody>
        </table>
    </div>
</template>


<style>
        .page-shopping-cart .td-product {
            width: 460px;
        }
        .page-shopping-cart .red-text {
            color: #000;
        }
        .page-shopping-cart .cart-product table {
            width: 100%;
            text-align: center;
            font-size: 14px;
        }
        .page-shopping-cart .cart-product table td {
            padding: 20px 0;
        }
        .page-shopping-cart .cart-product table tr {
            border-bottom: 1px dashed #e3e3e3;
        }
        .page-shopping-cart .cart-product table tr:last-child {
            border-bottom: none;
        }
        .page-shopping-cart .cart-product table .td-product {
            text-align: left;
            font-size: 12px;
            line-height: 20px;
        }
        .page-shopping-cart .cart-product table .td-product .product-info {
            display: inline-block;
            vertical-align: middle;
        }
</style>

<script>
export default {
     data () {
        return {
            productList: [
                {
                    pro_name: '标准票',
                    pro_purity: '',
                    pro_price: 199
                },
                {
                    pro_name: '站票',
                    pro_purity: '无座位,可自备小板凳...',
                    pro_price: 99
                },
                {
                    pro_name: '远程支持票',
                    pro_purity: '可获得活动PPT等资料',
                    pro_price: 9.99
                },
                {
                    pro_name: '赞助商',
                    pro_purity: '获得品牌露出机会,详情联系...',
                    pro_price: 999.99
                }
            ],
            
        }
    },
    
}
</script>
