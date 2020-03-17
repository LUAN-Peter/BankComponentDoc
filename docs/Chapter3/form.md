### Input输入框 ###
实现用户鼠标或键盘输入功能。  

```html
<s-input
    v-model = "value"
    background = "grey"
    :disabled = "false"
    :placeholder = "placeholder"
    label = "标签"
    prefixicon = "preicon"
    :prefixiconclick="handlePre"
    suffixicon = "preicon"
    :suffixiconclick="handleSuf"
    :ispassword = "true"
    errinfo = "错误信息"
    @blur="blur"
    @change="change"></s-input>
```  

```javascript
//头部和尾部图标需要引入，否则图片无法解析，可能是因为解析成String没有解析成url
import preicon from "../prefixurl/xx.png"       
import suficon from "../suffixurl/yy.png"
```

**属性**  


|  参数   | 说明  | 传入类型 | 参考值 | 默认值 |
|:----|:----|:---- |:----|:----|
| value  | 绑定的值(v-model) | String | - | - |
| disabled | 是否禁用 | Boolean | true/false | false |
| placeholder  | 占位文字 | String | - | - |
| label | 标签 | String | - | - |
| prefixicon | 头部图标url(注意import!) | String | - | - |  
| suffixicon | 尾部图标url(注意import!) |  String | - | - |
| ispassword | 显示密码文本 |  Boolean | true/false| false |
| ~~maxlength~~ | ~~最大输入文本长度~~ | ~~Number~~ | ~~-~~ | ~~-1(此时不限制)~~ |
| background | 输入框背景颜色 | String | white/grey | white |
| errinfo | 错误提示信息 | String | - | - |

>_maxlength样式不明确，搁置。_

**事件**  

| 名称 | 说明 | 回调参数 |
|:----|:----|:----|
| blur | 失去焦点时触发该事件 | Event($event) |
| input | 输入值时触发该事件 | Event($event.target.value) |
| prefixiconclick | 点击头部图标事件 | Event |
| suffixiconclick | 点击尾部图标事件 | Event |

**插槽**  

| 名称 | 说明 |
|:----|:----|
| suffix | 尾部插槽，不推荐和suffixicon同时使用，有待优化 | 


### Table表格 ###


### Select选择器 ###


### CitySelect城市选择器 ###


### DateSelect日期选择器 ###