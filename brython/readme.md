# readme
>  Brython is designed to replace Javascript as the scripting language for the Web

# 单元测试
```python 
# https://brython.info/tests/index.html?lang=en
import unittest

class IntegerArithmeticTestCase(unittest.TestCase):
    def testAdd(self):  ## test method names begin 'test*'
        self.assertEqual((1 + 2), 3)
        self.assertEqual(0 + 1, 2)
    def testMultiply(self):
        self.assertEqual((0 * 10), 0)
        self.assertEqual((5 * 8), 40)

suite = unittest.TestLoader().loadTestsFromTestCase(IntegerArithmeticTestCase)
unittest.TextTestRunner(verbosity=0).run(suite)
```

# 第三方库
http://brython.info/static_doc/en/import.html

# FAQ
http://brython.info/static_doc/en/faq.html

但是通过测试的功能，Brython通常比pypy.js更快，本身比Skulpt更快。在某些情况下，Brython比Python参考实现CPython更快。

# 例子
### py_hello
入门例子

### py_pyfile
因为有本地文件，需要启动server: python3 -m http.server 8000

http://127.0.0.1:8000/py_pyfile.html


### py_template
python写前端模版

注意open!

python3 -m http.server 8000

http://127.0.0.1:8000/py_template.html

# doc
https://brython.info/static_doc/en/intro.html?lang=en

# tips
asyncio能用



# 一些有趣的项目
*  [raphael python canvas](https://brython.info/gallery/raphael/basic.html)
*  [python three.js](https://brython.info/gallery/three.html)
*  [python vue](https://github.com/stefanhoelzl/vue.py)
*  [pyschool](http://pyschool.net/) 浏览器中学python，代码存在本地
*  [Deploying a Brython application](https://brython.info/static_doc/en/deploy.html)
*  [svg pie](http://brython.info/gallery/svg_pie_chart.html)
*  [turtle](http://brython.info/gallery/turtle.html): 直接使用python替代js，连用户输入都用python获取
*  [classroom](https://github.com/brython-dev/brython-in-the-classroom): 减少教师和学生访问python资源的负担