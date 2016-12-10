Listing
======

Listing是Product的集合，用于产品列表和搜索结果中显示一系列相关的Product。

例如在京东搜索一个iPhone，iPhone的不同颜色其实都是不同的Product，如果每个Product都占一个列表格子，列表就会变得很长，而且充满冗余。

我们希望把iPhone的各种颜色，容量都放到同一个产品页面里，用户进入产品页面之后再选择需要的款式，这个产品页面就是一个Listing。

Listing拥有名字，拥有一套各个Product合用的介绍文本，如果有需要的话介绍文本以后可以分到Product上，实现不同Product不同介绍。

Listing和Product是一对多关联，因为觉得一个Product在多个Listing里展示本身就属于冗余，而且引用关系相当难维护，所以直接关联了。

字段：

* name
* introduction