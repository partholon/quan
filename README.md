通信
  
  User
  1 当用户需要登录时，跳转到 _xxx_.php?url=url
    url为授权登陆后需要返回的地址
  2 授权成功后页面跳转到url?uid=uid
    uid为用户新浪uid
  3 获取用户资料接口 _xxx_.php?uid=uid  返回格式为json 如下
  {
  	"uid": 2687933660,  //uid
  	"name": "骛源归来不看花",  //用户昵称
  	"avatar": "http://ww2.sinaimg.cn/crop.0.102.612.612.1024/a0369cdcjw8ek8gtwklzpj20h00mowga.jpg", //用户头像
  	"gender": "女"
  }
  
  Market
  1 发布商品时ajax通过post请求_xxx_.php 参数
  {
  	"uid":2687933660, //发布者uid
  	"category":"代步工具",
  	"product_title":"自行车",
  	"price":"998",
  	"contacts":"哗哗哗",
  	"telephone":"110",
  }
