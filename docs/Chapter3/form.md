### Input输入框 ###
实现用户鼠标或键盘输入功能。  

```html
<s-input
    :value = "value"
    :placeholder = "placeholder"
    label = "标签"
    prefix-icon = "./test.png"
    suffix-icon = "./test1.png"
    :ispassword = "true"
    :maxlength = "10"></s-input>
```

**属性**  

|  参数   | 说明  | 传入类型 | 参考值 | 默认值 |
|:----|:----|:---- |:----|:----|
| value  | 绑定的值 | String | - | null |
| disabled | 是否禁用 | Boolean | true/false | false |
| placeholder  | 占位文字 | String | - | null |
| label | 标签 | String | - | null |
| prefix-icon | 头部图标url | String | - | null |
| suffix-icon | 尾部图标url |  String | - | null |
| ispassword | 显示密码文本 |  Boolean | true/false| false |
| maxlength | 最大输入文本长度 | Number | - | -1 |
| background | 输入框背景颜色 | String | white/grey | white |

**事件**  

| 名称 | 说明 | 回调参数 |
|:----|:----|:----|
| blur | 失去焦点时触发该事件 | ??? |
| suffix-icon-click | 点击尾部图标事件 | ??? |



***
### Table表格 ###

***
### Select选择器 ###

***
### CitySelect城市选择器 ###

***
### DateSelect日期选择器 ###