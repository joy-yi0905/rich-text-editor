# rich-text-editor
富文本编辑 

### 介绍

去年年初写的，主体内容采用iframe，功能见demo页。


### 为什么不用div代替iframe

- 当前文档的行为不会影响iframe中的元素。也就是说，当前页面定义的样式和js操作，对iframe中相同类名的元素是无效的。
- 对于文档操作，js提供了一套现成的execCommand方法。倘若我们用div来开发RTE，在没有现成方法的基础，那么就需要先提取选中的文字，然后再对选中的文字对象做处理，处理完后再获取光标位置，最后插入到对应的位置，这当中所涉及到的方法兼容性都一塌糊涂，而且方法名都很长，谁搞谁知道。


rich-text-editor演示：[点击查看](http://joy-yi0905.github.io/rich-text-editor/)
