---
title: threaded_comments property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 220
url: /python-net/aspose.cells/comment/threaded_comments/
is_root: false
---

## threaded_comments property


Gets the list of threaded comments;

### Example 


```python

threadedComments = comment1.threaded_comments
for i in range(len(threadedComments)):
    tc = threadedComments[i]
    note = tc.notes

```
### Definition:
```python
@property
def threaded_comments(self):
    ...
```

### See Also
* module [aspose.cells](../../)
* class [Comment](/cells/python-net/aspose.cells/comment)
* class [ThreadedCommentCollection](/cells/python-net/aspose.cells/threadedcommentcollection)
