### 3.1 文档：DOM中的『D』

当创建了一个网页并把它加载到Web浏览器中时，DOM就在幕后悄然而生了。它把你编写的网页文档转换为一个文档对象。

DOM把一份文档表示为一棵树。  可以称为“节点树”。![屏幕快照 2015-11-16 23.49.53](/Users/junfengli/Documents/JavaScript-DOM-2-/images/屏幕快照 2015-11-16 23.49.53.png) ![屏幕快照 2015-11-16 23.50.04](/Users/junfengli/Documents/JavaScript-DOM-2-/images/屏幕快照 2015-11-16 23.50.04.png) ![屏幕快照 2015-11-16 23.50.16](/Users/junfengli/Documents/JavaScript-DOM-2-/images/屏幕快照 2015-11-16 23.50.16.png)



### 3.4 节点

DOM有许多不同类型的节点，比如：元素节点、文本节点和属性节点。

#### 3.4.1 元素节点

DOM的原子是元素节点。

如果把Web上的文档比做一座大厦，元素就是建造这座大厦的砖块，这些元素在文档的布局形成了文档的结构。

标签的名字就是元素的名字。

文本段落的元素名字是“P”；无序清单元素的名字是“ul”；列表项元素的名字是“li”。

元素可以包含其他元素。

#### 3.4.2 文本节点

在上面的例子中，<p>元素包含文本“Don’t forget to buy this stuff.” 这段英文就是文本节点。

在XHTML文档里，文本节点总是被包含在元素节点的内部。但并非所有的元素节点都包含有文本节点。

#### 3.4.3 属性节点

属性节点用来对元素做出更具体的描述。

<p title="a gentle reminder">Don't forget to buy this stuff.</p>

`title="a gentle reminder"`是一个属性节点。

 ![屏幕快照 2015-11-22 23.23.56](/Users/junfengli/Documents/JavaScript-DOM-2-/images/屏幕快照 2015-11-22 23.23.56.png)

属性总是被放在起始标签里，所以属性节点总是被包含在元素节点中。

并非所有的元素都包含着属性，但所有的属性都被元素包含着。

#### 3.4.4 CSS（层叠样式表）

告诉浏览器应该如何显示一份文档。

类似JavaScript脚本，对样式的声明即可以嵌在文档的<head>部分（<style>标签之间），也可以放在另外一个样式表文件里。

CSS声明元素样式语法：

``` css
selector {
  property: value;
}
```

