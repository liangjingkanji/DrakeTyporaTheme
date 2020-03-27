## 介绍

最好的实时预览Markdown工具[Typora](https://typora.io/)使用的主题



1. 截图使用的字体: [JetBrainsMono](https://www.jetbrains.com/lp/mono/), 安装即可
2. 代码高亮配色来自JetBrains IDE



**建议使用加粗作为标识小标题**

代码渲染来自JetBrains公司的IDE`Darcula`主题

```kotlin
class MultiTypeFragment : Fragment() {

  override fun onCreateView(
    inflater: LayoutInflater, container: ViewGroup?,
    savedInstanceState: Bundle?
  ): View? {

    return inflater.inflate(R.layout.fragment_multi_type, container, false)
  }

  override fun onActivityCreated(savedInstanceState: Bundle?) {
    super.onActivityCreated(savedInstanceState)
		
    // 创建多类型RecyclerView列表
    rv_multi_type.linear().setup {
      addType<Model>(R.layout.item_multi_type_simple)
      addType<DoubleItemModel>(R.layout.item_multi_type_double)
      
      onClick(R.id.item) {
        when (itemViewType) {
          R.layout.item_multi_type_simple -> toast("类型1")
          else -> toast("类型2")
        }
      }
    }.models = getData()
    
  }
}
```



> 这是一个引用渲染样式预览



代码片段可以作为代码或者高亮显示`typora_theme_drake`

这是一个[超链接Google谷歌](https://github.com/liangjingkanji)



脚注样式示例[^Drake]



[^Drake]: 脚注一般情况不常用, 哈哈, `_drake`	

## 安装方式

复制`drake.css` 到`theme`目录下然后重启, 选择菜单栏主题

通过`设置 -> 外观 -> 打开主题文件夹`打开theme目录.

## 截图预览

![image-20200108132629294](https://tva1.sinaimg.cn/large/00831rSTgy1gd8mqxk4wlj30u017q17e.jpg)

