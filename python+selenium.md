## 准备环境
下载Chromedriver:  
https://sites.google.com/a/chromium.org/chromedriver/downloads    
添加环境变量  

## 测试框架  
### 框架基本组件   
1）配置文件和全局环境变量      
2）框架主要代码：包含日志类，自定义封装基类，配置文件读取以及各种调度    
3）产品业务页面：业务页面，业务逻辑分层，分页独立出来   
4）测试脚本集合：考虑采用第三方单元测试框架来管理和创建测试单元      
5）日志和报告：测试报告和日志文件输出，报告可能要借助第三方插件     
6）第三方插件引入    
7）持续集成：比如jenkins   

## Unittest
创建Python Unittest  
case名以test打头  
import unittest，selenium.webdriver模块  
class继承unittest.TestCase   
最后结尾处的unittest.main(),添加这个是支持在cmd里面，cd到这个脚本文件所在的目录，然后Python 脚本名.py执行，如果不添加这一段，是无法执行cmd里面运行脚本的    
### 测试固件（test fixture）   
setUp()和tearDown()    

### 测试用例（test case）     
unittest中管理的最小单元是测试用例，一个测试用例，包括测试固件，和具体测试业务的函数或者方法。   

### 测试套件 （test suite）     
就是很多测试用例的集合    

### 测试执行器 （test runner）     
用来执行加载测试用例，并执行用例，且提供测试输出的一个组建。    

### POM   
把web ui对象仓库从测试脚本分离，业务代码和测试脚本分离。     


## selenium  
### 基本概念   
元素  
在网页上面的文本输入框，按钮，多选，单选，标签，和文字都叫元素，总之，凡是能在页面显示的对象都可以作为页面元素对象。
  
元素定位  
一个网页元素，也有位置，可以通过一些手段或者表达式去描述这个元素在页面对应的位置。   
   
XPath  
它是一种用来确定XML文档中某部分位置的语言。  
Selenium一共有八种元素定位方法，其中，在实际开发自动化脚本过程中，XPath的使用是最多的一种方法。  

### xpath
### innerHTML
### 访问元素HTML属性
get_attribute()  

