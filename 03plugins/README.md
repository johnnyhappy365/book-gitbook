# 插件

以下介绍几个我尝试或正在使用的插件

## disqus 评论插件

安装插件

```bash 
npm install gitbook-plugin-disqus -g
```

修改book.json

```json
{
    "plugins": ["disqus"],
    "pluginsConfig": {
        "disqus": {
            "shortName": "book-gitbook"
        }
    }  
}
```

## theme-score 主题插件

默认的主题是黑白的，加上这个主题会好看一些。book.json中增加这个配置，然后 `gitbook install` 就可以了
```json
"plugins": [theme-comscore"],
```

执行 `gitbook install` 进行插件安装，然后运行 `gitbook serve` 启动。

## 没有银弹

disqus在国外使用效果非常好，国内就没有一个可以的插件了。还有一种方案是把评论提交到github issue上，但这对程序员还行。其它用户使用起来就不是很友好了。

## prism 代码样式
prism: 为代码增加更好看的样式。但需要把默认的插件屏蔽掉。


```json
"plugins": [
  "prism",
  "-highlight"
],
"pluginsConfig": {
  "prism": {
    "css": [
      "prismjs/themes/prism-solarizedlight.css"
    ],
    "lang": {
      "shell": "bash"
    }
  }
}
```

## copy-code-button 复制代码

```json
"plugins": [
  "copy-code-button"
]
```

## 其它参考

http://gitbook.zhangjikai.com/plugins.html