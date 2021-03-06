# 1 伪类和伪元素

- **伪类**：其核心就是用来选择那些不能够被普通选择器选择的文档之外的元素，比如:hover。

  |     选择器      |                             作用                             |
  | :-------------: | :----------------------------------------------------------: |
  |     :active     |               匹配被用户激活的元素（比如点击）               |
  |     :focus      |                     匹配获取焦点的的元素                     |
  |    :checked     |                匹配被选中的radio或者checkbox                 |
  |    :disabled    |                匹配处于不可用状态的可交互元素                |
  |  :first-child   |                匹配在兄弟元素中处于第一的元素                |
  | :first-of-type  |        匹配在它的兄弟元素中是某个类型中的第一个的元素        |
  |     :hover      |                匹配用户在此悬停或者触摸的元素                |
  |  nth-child(n)   | 匹配父元素的第n个子元素。n可以是一个数字、一个关键字或一个公式 |
  | :nth-of-type(n) | 匹配父元素的某种类型元素中的第n个子元素。n可以是一个数字、一个关键字或一个 公式 |

- **伪元素**：其核心就是需要创建通常不存在于文档中的元素，比如::before。



|     选择器     |                  作用                  |
| :------------: | :------------------------------------: |
|    ::before    | 匹配在原始元素的实际内容之前出现的区域 |
|    ::after     | 匹配在原始元素的实际内容之后出现的区域 |
| ::first-letter |          匹配元素的第一个字母          |
|  ::first-line  |             匹配元素第一行             |
|  ::selection   |        匹配被选中的文本或者区域        |



# 2 flex中的flex: 0 1 auto是什么

### 2.1 flex-grow

**表示当子元素的空间小于父元素的空间时,如何处理剩余空间**,
默认值为0表示不占有剩余空间;
当子元素都设置为1时表示平均分配剩余空间;
当一个子元素为2其余子元素为1时为2的子元素占据的剩余空间比其他子元素多一倍;
当一个子元素为1其余子元素为0,为1的子元素占据全局剩余空间

### 2.2 flex-shrink

**表示当子元素的空间大于父元素的空间时,如何缩小子元素**
默认值为1表示等比缩小
当所有子元素都设置为1时所有子元素都会等比例缩小
当一个子元素为0其余子元素为1是表示为0的子元素不缩小,其余元素缩小

### 2.3 flex-basis

**用于设置项目占据的主轴空间**,设置为auto表示项目占据的主轴大小等于项目的实际内容大小,设置为固定值表示项目占据的主轴大小等于固定值。



# 3 CSS实现三角形

``` css
.triangle {
    width: 0;
    height: 0;
    border-top: 50px solid black;
    border-right: 50px solid transparent;
    border-left: 50px solid transparent;
}
```



# 4 CSS实现扇形

``` css
.round {
    width: 100px;
    border: 50px solid transparent;
    border-right-color: red;
    border-radius: 50%;
}
```

