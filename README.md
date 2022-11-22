# 收款二维码合并  
## 原理
扫描二维码后跳转到此页面，然后根据 UA 判断具体平台。  
支付宝为:AlipayClient  
微信为:MicroMessenger  
然后根据平台进行跳转，支付宝可以直接跳转到收款链接，而微信只能跳转到二维码进行付款。  
同理可以添加其他平台的支付方式。  
## 配置
### 1.更换支付宝收款链接  
保存支付宝收款二维码，使用二维码识别软件进行识别，得到链接。  
**得到的链接是大写的，不要进行任何处理或转换成小写**  
然后将 index.html 中的变量 alipayURL 改为自己的支付宝收款链接。
### 2.更换微信二维码
保存微信收款二维码，放到 static/ 文件夹中，并命名为 wechat.png  
### 3.添加 QQ 二维码(可选项)   
将 QQ 收款二维码放到 static/ 文件夹中,并命名为 qq.png   
将 index.html 中的 qqSwitch 改为 true(相应地,不使用的同学请将其改为 false)   
### 4.添加 TIM 二维码(可选项)   
将 TIM 收款二维码放到 static/ 文件夹中,并命名为 tim.png   
将 index.html 中的 timSwitch 改为 true(相应地,不使用的同学请将其改为 false)   
### 3.设置为 Github Pages
选择 Settings --> GitHub Pages 设置为 Github Pages  
**如果没有通过 ICP 备案的域名建议不要使用自定义域名，会被微信拦截**  
设置成功后得到链接，使用链接生成二维码即可。   


欢迎 pr 或 issue.   

__弃坑__ 
