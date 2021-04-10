这是用来解决什么问题的? 是用来解决某些文件, spotlight默认不会索引, 但它们其实就是平文本, 比如.rs, 比如.Rmd, 比如.R

1. 首先需要用automator创建一个新的空的应用, 不妨取名为dummy
2. 修改dummy的Info.plist
3. 修改/System/Library/Spotlight/RichText.mdimporter/Contents/Info.plist, 需要与第2步的修改匹配

具体2,3怎么改, 看repo中对rust的处理(.rs)

其实我也不确定2,3中每一步都是必要的. 而且似乎这个设置不会立即生效. 我曾经折腾了一晚上, 不行, 过了好几周(也可能只需要好几天), 自动就生效了. 我怀疑, 是不是需要登出再login就行了
