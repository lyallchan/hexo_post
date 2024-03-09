# 折腾手记

使用hexo生成静态博客，托管在[github](http://lyallchan.github.io)

# 使用环境

安装好nodejs和cnpm，可以参考这篇[文章](http://lyallchan.github.io/2015/12/10/%E5%AE%89%E8%A3%85%E5%92%8C%E9%85%8D%E7%BD%AEnvm%E3%80%81nodejs%E5%92%8Chexo/)

```bash
cnpm install hexo-cli -g
git clone git@github.com:lyallchan/blog_src.git blog
cd blog
cnpm install 
```

# 增加文章和发布

直接在source/_post下新建md文件，然后hexo generate和deploy

```bash
cd blog
hexo d -g
```

