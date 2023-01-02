
# 基础教程

`*`表示为拓展语法,仅在Typora或添加了拓展的VScode本地生效,在大多数平台上并不认可

# 0. 写Markdown的第零步

我们在写文本的时候大多时候写的是中文,但是中文输入法使用的标点符号为全角标点, 如，。？！（）【】：；“” . 这些标点是不被markdown所认可的, 也就是无法转意的.  
我建议大家写Markdown的时候都用半角标点,如,.?!()[]:;"". 且每个半角标点在文本使用时加上后置空格,符合英文标点的书写规范也更美观

# 1. 标题[数个"#"+空格+标题名字]

```text
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题(可能有地方不支持)
```

标题会在目录与大纲分级显示,可以跳转.
在Typora中建议开启**严格模式**,即不应为 **#标题**,应为 **# 标题**  
应当手动补上空格,使得markdown语法在其他编辑器或查看器上兼容.
标题上下应当有一个空行,否则lint会出错,而且不应当跳过标题级别

# 2. 强调[用"**"或"__"包围]

**欢迎报考南京大学!**  
**再次欢迎**  
**建议全局使用统一的强调符号**
或者选中想要强调的文字按下**Ctrl+B**

# 3.斜体[用"*"或"_"包围]

或者选用想要强调的文字按下**CTRL+I**  
*欢迎各位大佬来焦焦我各种知识*
***还可以套娃,这是强调+斜体***

# 4. 删除线[用"~~"包围]

~~我宣布个事,我是shabi!~~

# 5. *高亮[用"=="包围]

==(注意:此为拓展语法)==
很明显vscode的markdown all in one拓展不支持,git也不支持

# 6. 代码[用"```"包围]

```c++
//在第一个```的上方应当留出空行,且应当在第一个```的后方指定语言,如test(文本)
//c++, java, etc
int main(){  
    printf("hello world");  
}
//在第二个```的下方应当留出空行
```

还有一个方法:  
直接使用四个空格(TAB)缩进表示代码块,但是整个md中应当**保持一致**,否则lint会出错  

# 7. 引用[">"+空格 前置]

> 24岁,是学生  
> > 学生特有的无处不在  

引用是可以嵌套的,引用完成后应当加上空行

# 8. 无序列表["-"或"+"+空格 前置]

- 一颗是枣树  
- 另外一颗还是枣树  
  - 按一下TAB可以变为引用的子集
引用完成后也需要加空行

# 10. 有序列表[数字+"."+空格]

1. 一颗是枣树
2. 另一颗还是枣树

完成之后需要空行

# 11. *上标[用"^"包围]

C语言中int的上限是2^32^ - 1 = xxxx
很明显vscode的这个拓展也不支持这玩意,我去git试试,经过测试,git也不支持

# 12. *下标[用"~"包围]

H~2~O是剧毒的!

# 13. *注释["[^]"]后置

这是一个注释[^]  
这是一个脚注[^1]  

[^1]真正的脚注  

# 14. 链接[常用"[]"+"()"分别包围文本与链接]

(注意:文内跳转为拓展用法)  
[来看看我贫瘠的仓库](https://github.com/Ckkyo/learn_markdown#readme)  
[基础教程:12. 下标](#12. *下标[用"~"包围])  
很明显文内跳转也不能用  

# 15. 任务列表["-空格[空格/x]"+空格 前置]

```text
-[ ] 刷B站  
```

- [ ] 刷B站  
- [X] 刷过了

# 16. 表格[用"|"绘制表格边框]

```text
| 学号 | 姓名 | 年龄 |  
| :--- | :---: | ---: | (冒号的位置代表着 左对齐,区中,右对齐,中间的-可以任意个)
|123|猫猫头|24|
```

| 学号 | 姓名 | 年龄 |  
| :-- | :--: | --: |
|123     |猫猫头|24|  
|124|复读机|100|

# 17. 图片[直接拖进来或者复制粘贴]

file:///home/ck/do_sth_here/learning/markdown/img/ec43126fgy1h1y47yuiy5j212l1fekjl.jpg

file:https://github.com/Ckkyo/learn_markdown/tree/main/img/ec43126fgy1h1y47yuiy5j212l1fekjl.jpg


ec43126fgy1h1y47yuiy5j212l1fekjl.jpg