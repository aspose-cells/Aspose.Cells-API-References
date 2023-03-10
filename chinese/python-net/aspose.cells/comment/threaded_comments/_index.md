---
title: threaded_comments 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 220
url: /zh/python-net/aspose.cells/comment/threaded_comments/
is_root: false
---
## threaded_comments 属性

获取线程评论列表；

### 例子

```python

threadedComments = comment1.threaded_comments
for i in range(len(threadedComments)):
    tc = threadedComments[i]
    note = tc.notes

```
### 定义：
```python
@property
def threaded_comments(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Comment](/cells/zh/python-net/aspose.cells/comment)
* 类 [ThreadedCommentCollection](/cells/zh/python-net/aspose.cells/threadedcommentcollection)
