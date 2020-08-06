## 介绍



1. 截图使用默认的字体: [JetBrainsMono](https://www.jetbrains.com/lp/mono/), 安装即可. 如果需要自定义字体修改CSS文件`第11行`字体名称即可替换全部字体
2. 代码渲染配置来自`JetBrains Darcula`
3. 脚注样式来自于`维基百科`





## 安装方式

1. 首先确定已安装 [Typora](https://typora.io/)

2. 复制`drake.css` 到`theme`目录下然后重启, 选择菜单栏主题

3. 通过`设置 -> 外观 -> 打开主题文件夹`打开theme目录



**加粗效果**

```kotlin
override fun onCreate(savedInstanceState: Bundle?) {
    super.onCreate(savedInstanceState)
    setContentView(R.layout.activity_main)

    state.onRefresh {
        // 一般在这里进行网络请求
        thread {
            Thread.sleep(2000)
            showContent()
        }
    }.showLoading()
}
```



这里演示脚注内容[^2]



> 推荐用于醒目标注内容



[^2]: 脚注内容, 一般不使用脚注因为很多文档不支持Markdown脚注渲染(例如GitHub不支持脚注)

## 截图预览

![image-20200802050022271](https://i.imgur.com/J34NMr6.png)


