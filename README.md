# 草榴种子下载器

项目依赖Python3,需要requests库。国内运行需要翻墙。此项目仅用于代码学习

打开Caoliu.py，最后几行如下:
```python
if __name__ == "__main__":
c = Caoliu()
c.index_page()
c.start(type="yazhouwuma",page_start=1,page_end=20,max_thread_num=50)
```
type参数负责下载类型，其对应如下:
|下载类型|type|
|:--:|:--:|
|亚洲无码|yazhouwuma|
|亚洲有码|yazhouyouma|
|欧美原创|oumeiyuanchuang|
|动漫原创|dongmanyuanchuang|
|国产原创|guochanyuanchuang|
|中字原创|zhongziyuanchuang|

page_start,page_end代表起始页和终止页
max_thread_num代表允许程序使用的最大线程数
设定好各参数后，运行Caoliu.py。会在目录下创建一个torrent_dir，并开始下载种子。
![image1](https://raw.githubusercontent.com/chuxiuhong/cloudphoto/master/1024.png)



