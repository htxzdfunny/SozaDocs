# 关于 

## 直接为 Cytoid wiki 作出贡献

### 格式规范

如果您直接在GitHub提交更改(pull request), 那您必须遵守以下规范

1. 格式: 使用Markdown(docsify增强版)进行编辑
2. 标点: 应当使用英文标点的地方按英文电子书面习惯使用英文标点, 原本使用全角标点(中文标点)的使用英文标点并在标点后加空格(需要紧凑布局时可不加空格)
3. 板式: 文章内应合理地, 有逻辑地留出空行
4. 资源引用: 在同级文件夹中新建文件夹`_source_文章名.md`(注意,这是个文件夹,是有后缀的,根据docfify的奇妙特性,引用请`[!](/_source_文件名.md/file)`)
5. 内容: 使用Cytoid已经获得授权的内容
6. 署名: 请在文章末尾或开头中合适位置署名,格式: `!> 作者: Li Ming`
7. 其他: 文章名请不要与现有文章冲突

如果您选择用issues的方式提交您的文章, 则无需遵守, 我们会对您的文章进行格式修正, 但提交时请将资源打包成zip发送

编辑时**显示效果**为重, 统一性在后. 例如: 

> 刚入门Cytoid? 不妨试试Cytoid自带的官方谱面
>
> Cytoid 非常愿意与艺术家进行合作, 为玩家提供优秀的游戏体验. 

第二句需要突出主语, 因此与后面字符有一个空格

本规范并非强制性, 本身也在不断修正, 您在参考的同时也能提出异议

[support](../site-source/part/support.md ':include')

### 特殊格式

!> docsify中, `/`指的是当前位置, 上一级需要`../`, 再上一级要`../../`

本 wiki 魔改过部分渲染内容, 例如: 

~~~
![Palescreen](../../site-source/pic/backgrounds/palescreen.jpg ":class=side-img")
~~~

![Palescreen](../../site-source/pic/backgrounds/palescreen.jpg ":class=side-img")

会渲染成

~~~
<div class="side-img">
    <img src="/zh/about/../../site-source/pic/backgrounds/palescreen.jpg" alt="Palescreen">
    <p>Palescreen</p>
</div>
~~~
如右图


