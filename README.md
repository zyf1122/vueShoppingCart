#vue购物车练习

###项目主主体分两页,使用vue2.0和axios,数据为本地模拟的就送数据

#####cart(购物车页)

- 一打开网页,使用mounted钩子函数直接发送网络请求,获取购物车列表数据
- 使用v-for循环,遍历渲染数据
- 点击+/-按钮,实现商品数量加/减,运用v-model特性,实现单类商品总价格随之更改
- 点击勾选按钮,实现所有总商品价格的计算,使用$set给接受的数据对象里添加一个checked属性,来检测是否勾选了
- 定义一个data里的属性来记录点击的循环的那类商品,然后找到它的索引,来操作列表数据,以实现删除功能(一般通过发送请求给后台,后台返回状态码,确认是否删除了)
- 定义过滤器,对价格数据进行格式化

#####address.html(收货地址页)

- 一点击结算,打开收货地址网页,使用mounted钩子函数直接发送网络请求,获取地址列表数据
- 使用v-for循环,遍历渲染数据,定义过滤器,对数组进行过滤,只显示前三组数据,点击more,改变过滤的长度,显示全列表
- 击时将当前地址index赋值为此列表项的地址ID,实现当前的项选中,其他项未选中功能
- 收费选项同上,互斥
- 删除按钮同购物车页面(省略)
- 编辑按钮点击跳转到新页面,一个form表单页(省略)

![image](https://raw.githubusercontent.com/he1237596/vueShoppingCart/master/1.gif)
![image](https://raw.githubusercontent.com/he1237596/vueShoppingCart/master/2.gif)
