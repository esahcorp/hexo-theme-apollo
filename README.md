![hexo-theme-apollo](https://cloud.githubusercontent.com/assets/9530963/13026956/08e76eca-d277-11e5-8bfc-2e80cea20a0d.png)

## 文档

- [中文文档](https://github.com/esahcorp/hexo-theme-apollo/blob/master/doc%2Fdoc-zh.md)
- [Document](https://github.com/esahcorp/hexo-theme-apollo/blob/master/doc%2Fdoc-en.md)

## 安装

[![asciicast](https://asciinema.org/a/emrvroa9054hz6k8ise0uxh2u.png)](https://asciinema.org/a/emrvroa9054hz6k8ise0uxh2u)

``` bash
hexo init Blog 
cd Blog 
npm install
npm install --save hexo-renderer-jade@0.30 hexo-generator-feed hexo-generator-sitemap hexo-browsersync hexo-generator-archive
git clone https://github.com/esahcorp/hexo-theme-apollo.git themes/apollo
```

注意由于 jade 包更名为 pug，最新的 hexo-renderer-jade 包已经无法处理 /layout 中的 .jade 文件，需要指定版本为 @0.30

## 启用

修改博客根目录下的 `_config.yml` 的 `theme` 配置项为 `apollo`:

```yaml
theme: apollo

# 在归档页面显示所有文章
# 需要上面安装的 hexo-generator-archive 插件支持
archive_generator:
    per_page: 0
    yearly: false
    monthly: false
    daily: false
```

hexo 默认的链接方式为 /年/月/日/文章名，可以在根目录下修改 `permalink`

```yaml
# 修改为 /年/文章名 的格式
permalink: :year/:title/
```

## 更新

``` bash
cd themes/apollo 
git pull
```

## License

MIT
