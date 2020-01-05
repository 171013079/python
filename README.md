#### 此作业共制作了7个页面
* [pythonanywhere地址](http://rangerb1.pythonanywhere.com/)

每个页面都能够正常加载的 只是需要时间较长 图表反映也较慢，请耐心等候。
#### 一、 github文档（templates、static、app.py、数据文档）
上述文档都存放在github页面中，请上移页面查看。
![](https://upload-images.jianshu.io/upload_images/9540329-ebd84f28af60c707.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 二、 技术文档书写
所有的HTML文件放置在templates文件夹中，其中base.html和results2为最基础模板，没有内容。内容都在p1-p7页面内。
![](https://upload-images.jianshu.io/upload_images/9540329-838aed3cb373db6f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

每页对应不同的hmtl内容，其中每页都设置了对应的跳转：
例如p1：![p1](https://upload-images.jianshu.io/upload_images/9540329-893d098bdf5708ef.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 三、Python档描述 
* 安装并导入pandas、pyecharts、cufflinks、plotly等第三方包
![](https://upload-images.jianshu.io/upload_images/9540329-8ed353011a3fbb6a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* pandas读csv文件
![](https://upload-images.jianshu.io/upload_images/9540329-9ef39c6bcdb092ef.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
（文件内路径与pythonanywhere不同）
* pyecharts的模块画散点、条形图等，并将部分图以html文件的方式导出
* 安装Flask环境，导入flask和render_template函数。

* methods (GET、POST)
![](https://upload-images.jianshu.io/upload_images/9540329-4a8832c04c13b053.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


视图函数 def
根据不同页面的不同功能写函数。如传入与返回
![](https://upload-images.jianshu.io/upload_images/9540329-8ccc383cb2854b55.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#### 四·、Web App动作描述
1.  后端伺服器启动：执行 app.py 启动后端伺服器，等待web请求。启动成功应出现：* Running on [http://127.0.0.1:8040/](http://127.0.0.1:8040/) ![image.png](https://upload-images.jianshu.io/upload_images/9540329-1b335eddc7bf6d9c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2.  前端浏览器web 请求：访问端口，启动前端web 请求
3.  后端伺服器web 响应：py文件执行 了@app.route('/') 下的 index()函数，响应对应路径的页面
4. 前端浏览器收到web 响应：出现网页，其中一些页面有表单的输入 input 类型为"SUBMIT"，web接收到请求后，则产生新的web 。

#### 五、用到的部分代码内容：
运用到列表循环，for循环等等<br>
运用到数据结构嵌套适合在子页面中嵌套出现数据交互图和数据图表<br>
利用推导式使得在子页面中进行不同html的跳转<br>
利用判断语句判断用户点击的是什么从而跳转到相应界面<br>
在python档中赋予不同html文件不同的跳转地址并且开展出不同功能，实现python文档与html文档的数据交互(type) <br>
提供app.py档以供查看：[app.py]([https://github.com/171013079/python/blob/master/app.py)
#### 六、页面简述：（由于需要截图的问题，页面缩放观感较差）
* p1：显示主题内容：日益变胖的地球人，页面上方设有下一页按钮，可以进一步查看数据与图表
![](https://upload-images.jianshu.io/upload_images/9540329-8dc979b7b73568ba.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* p2:  主题为：2018年世界人口BMI平均指数，页面显示plotly的可视化世界地图，页面上方有下一页按钮。
![](https://upload-images.jianshu.io/upload_images/9540329-333d6636b855b177.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



* p3:同上，图表内容为世界地区肥胖症发生率，  在之前页面的基础上做了下拉选框 数据内容会随着选框选择变化而变化。
![image.png](https://upload-images.jianshu.io/upload_images/9540329-0764848edc48db9b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


* p4:图表主题为：不同发展国家由于超重而引发的患病率分析。用了tab栏，可切换图表内容。
![](https://upload-images.jianshu.io/upload_images/9540329-e948bfc221306c77.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* p5：图表主题为：肥胖是早期死亡的主要危险因素之一
![image.png](https://upload-images.jianshu.io/upload_images/9540329-0f82c9b0b2e012f1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* p6/ p7：此页面大致同上，不再赘述。


（ps：其中每页都用了css技巧，为每页背景添加了颜色，有些页面为了更好的观感则选择了文字居中。）
