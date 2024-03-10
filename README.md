# 折腾手记

使用hexo生成静态博客，托管在[github](http://lyallchan.github.io)

# 使用环境

安装好nodejs和cnpm，可以参考这篇[文章](http://lyallchan.github.io/2015/12/10/%E5%AE%89%E8%A3%85%E5%92%8C%E9%85%8D%E7%BD%AEnvm%E3%80%81nodejs%E5%92%8Chexo/)

```bash
git clone git@github.com:lyallchan/hexo_post.git blog
cd blog
npm install 
```

# 增加文章和发布

直接在source/_post下新建md文件，然后hexo generate和deploy

```bash
cd blog
hexo d -g
```

# 如果需要从头安装

```bash
mkdir blog
cd blog
npx hexo init
npm install hexo-deployer-git --save
npm install hexo-theme-next@7.8.0 --save
npm install hexo-simple-image --save
git init
cp _config.yml _config.next.yml .gitignore 拷贝配置文件
git add . 
git commit -m "Update"
git remote  add origin git@github.com:lyallchan/hexo_post.git
git push --set-upstream origin main
```
