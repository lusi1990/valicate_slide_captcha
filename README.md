# 滑块验证码思路

参考资料:

* [使用 Python + Selenium 破解滑块验证码](https://www.aneasystone.com/archives/2018/03/python-selenium-geetest-crack.html) 
* ~~[python selenium 淘宝滑块验证码 问题](https://www.jianshu.com/p/afdabf486b54)~~
* ~~[修改 chromedriver key](https://stackoverflow.com/questions/33225947/can-a-website-detect-when-you-are-using-selenium-with-chromedriver)~~
* [Python + selenium 如何绕过爬虫特征检测](https://www.fengzifz.com/2021/06/17/hide-python-selenium-spider-feature/)
 
## PS: 

如果不想被检测到是 selenium 控制的浏览器可以添加参数 options.add_experimental_option('excludeSwitches', ['enable-automation']), 启用开发者模式.
现在还需要添加 `options.add_argument('--disable-blink-features=AutomationControlled')`


但是通过浏览器指纹仍然可以被检测到是爬虫
