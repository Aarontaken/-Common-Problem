# 动态改变列表中条目的宽高
需求：将一条广告插入一个医生列表中，广告高度和医生条目高度相同
思路：listview刷新填充数据之后，计算listview中医生条目高度，设置给广告条目并刷新。

改需求：这样的做广告会拉伸或压缩，给广告一个固定的宽高比scale，使其不再变形
思路：给广告图片设置addOnGlobalLayoutListener,根据scale和ImageView的宽度计算高度。
