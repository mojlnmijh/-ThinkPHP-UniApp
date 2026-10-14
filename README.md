# 全开源点餐系统源码ThinkPHP+UniApp
获取源码：ym7k.com/17837/
一、技术栈先看版本
组件	要看什么	风险
ThinkPHP	TP6/8 才在维护	TP5 已停更，安全漏洞多
UniApp	Vue2 还是 Vue3	Vue2 生态老，Vue3 兼容要验
PHP	7.4+ / 8.0+	太低跑不动
后台	FastAdmin / Vue	部分插件收费
二、“全开源”验什么
核心文件是否加密：application、vendor、extend 里搜加密文件。

授权回调：有没有远程验证，跑路后系统瘫痪。

后门：搜 eval、base64_decode、assert、异常外链、隐藏管理员。

前端源码：UniApp 给的是源码还是编译包。

License：MIT/Apache 真开源，还是“购买后可用”。

三、点餐系统重点验八块
模块	验收点
门店	单店/多店、总部+门店权限
商品	分类、规格、库存、沽清
点餐	桌码、扫码点餐、加菜、叫号
订单	下单、支付、退款、按门店分流
后厨	云打印机对接（飞鹅/易联云等）
收银	补单、结账、退款、小票、钱箱、扫码枪
分账	多店是否走官方分账，别二清
多端	微信/支付宝/抖音支付登录是否真跑通
四、最常见的坑
加密文件：号称全开源，核心逻辑加密。

授权回调：远程验证，跑路后系统瘫痪。

多端缩水：只有微信真跑通，支付宝/抖音是空的。

分账是二清：多店代收代付没走官方分账，违法。

打印机对接不全：只支持某品牌，或额外付费。

沽清/库存是假的：卖完不自动下架。

旧版改名：号称“最新版”，实际停更多年。

文档滞后：版本更新快，文档跟不上。<img width="1080" height="2340" alt="2025081609013543" src="https://github.com/user-attachments/assets/4f4d82ac-32c6-4bdb-9114-7148a594aa89" />
<img width="1080" height="2340" alt="2025081609004548" src="https://github.com/user-attachments/assets/b8175ce9-876c-46d5-a2bc-6abf0bacab37" />
<img width="1878" height="922" alt="2025081609020815" src="https://github.com/user-attachments/assets/e842f856-93b3-4cc1-a089-116b965f1789" />
<img width="1878" height="922" alt="2025081609020312" src="https://github.com/user-attachments/assets/1f78fead-4ff3-471b-96d3-0459bc4eb919" />
