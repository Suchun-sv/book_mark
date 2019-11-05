最近有需求，想不带书只带ipad上课，但是下载的pdf都是扫描版本，目录都不全，所以开动脑筋。
0. 实现效果![在这里插入图片描述](https://img-blog.csdnimg.cn/20191105143801638.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1N1Y2h1bnN2,size_16,color_FFFFFF,t_70)步骤：
1.  首先下载工具[Freepic2pdf](http://fastsoft.onlinedown.net/down/FreePic2Pdf.zip) 在这里感谢作者马健大大

	![在这里插入图片描述](https://img-blog.csdnimg.cn/20191105144015779.png)
2. 打开文件，我们要的只是更改pdf这一项
3.![在这里插入图片描述](https://img-blog.csdnimg.cn/20191105144137351.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1N1Y2h1bnN2,size_16,color_FFFFFF,t_70)
先取书签
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191105144201578.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1N1Y2h1bnN2,size_16,color_FFFFFF,t_70)
再开始骚操作：
下载[天若ocr](https://tianruoocr.cn/) 把pdf的目录给ocr了,这里同样感谢天若的作者，没找着名字，之后再补充感谢吧，哈哈哈
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191105144416233.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1N1Y2h1bnN2,size_16,color_FFFFFF,t_70)
ocr出来的是无格式的文件（没有缩进），之后自己用python写一个[脚本](https://github.com/Suchun-sv/book_mark)转换一下
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191105144734710.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1N1Y2h1bnN2,size_16,color_FFFFFF,t_70)
然后在复制替换导出的书签的那个文件，最后在倒回去就大功告成！是不是很简单。技术性的活动比如对页码加偏执之类的可以再转换的脚本里面改，很简单，就不赘述了。