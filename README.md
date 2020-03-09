# simple_spider
### 模块功能
#### 1.URL管理器负责管理URL链接，维护已经爬取的URL集合和未爬取的URL集合，提供获取新URL链接的接口。<br>
> 判断是否有待取的URL，方法定义为has_new_url()。<br>
> 添加新的URL到未爬取集合中，方法定义为add_new_url(url),add_new_urls(urls)<br>
> 获取一个未爬取的URL，方法定义为get_new_url()<br> 
> 获取未爬取URL集合的大小，方法定义为new_url_size()<br> 
> 获取已经爬取的URL集合的大小，方法定义为old_url_size()<br>
#### 2. HTML下载器用于从URL管理器中获取未爬取的URL链接并下载HTML网页。<br>
> 实现down_load(url)<br>
#### 3. HTML解析器用于从HTML下载器中获取已经下载的HTML网页，并从中解析出新的URL链接交给URL管理器，解析出有效数据交给数据存储器。<br>
#### 4.数据存储器用于将HTML解析器解析出来的数据通过文件或者数据库的形式存储起来。<br>
