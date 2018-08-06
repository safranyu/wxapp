# wxFlex布局
微信小程序的Flex布局demo－4种必备常用的Flex布局模式
## 官方建议的Flex布局
>Flex的布局相比传统的float布局来说，简单、快捷、方便。掌握flex布局可以在制作微信小程序时减少wxss的代码，同时也符合微信小程序开发的文档要求
本代码中涉及到四种Flex的布局方式，分别使用了不同的flex的不同属性。 建议看本文最后的学习参考进行相关属性的学习
## 骰子布局
>骰子布局中主要强调几个属性的使用```display ``` ```justify-content``` ```align-items ``` ```align-self``` 等
```
.dice_one{
  display: flex;
  justify-content: center;
  align-items: center;
}

.dice_two{
  display: flex;
  justify-content: space-between;
}
.dice_two .dice_item:nth-child(2){
  align-self: flex-end;
}
```
## 网格布局
>主要依赖flex属性，平均分布，需要设置自动缩放。
```
.Grid-cell {
  flex:1;
  
}
.Grid-cell-auto{
  flex: 2;
}
```
## 百分比布局
```
.cell-auto{
  flex: auto;
}
.cell-1of4 {
  flex: 0 0 25%;
}
```
## 流式布局
>每行项目会自动分行
```
.parent{
  display: flex;
  flex-flow: row wrap;
}
```
