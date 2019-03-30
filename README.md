![hexo-theme-simple](https://personal-1251959693.cos.ap-chengdu.myqcloud.com/2019-03-30-%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202019-03-30%2010.46.55.png)

## 文档

- [中文文档](https://github.com/Tit1e/hexo-theme-simple/blob/master/doc%2Fdoc-zh.md)
- [Document](https://github.com/Tit1e/hexo-theme-simple/blob/master/doc%2Fdoc-en.md)

## 贡献

该项目不再接受添加新特性、功能的 pull request，所有创造性的想法请 fork 该项目之后自由发挥。

## 安装

``` bash
hexo init Blog
cd Blog
npm install
npm install --save hexo-renderer-jade hexo-generator-feed hexo-generator-sitemap hexo-browsersync hexo-generator-archive
git clone https://github.com/Tit1e/hexo-theme-simple.git themes/simple
```

## 启用

修改 `_config.yml` 的 `theme` 配置项为 `simple`:

```yaml
theme: simple

# 在归档页面显示所有文章
# 需要上面安装的 hexo-generator-archive 插件支持
archive_generator:
    per_page: 0
    yearly: false
    monthly: false
    daily: false
```

## 更新

``` bash
cd themes/simple 
git pull
```

## License

MIT
