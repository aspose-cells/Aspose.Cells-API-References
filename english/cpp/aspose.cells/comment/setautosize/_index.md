﻿---
title: Aspose::Cells::Comment::SetAutoSize method
linktitle: SetAutoSize
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Comment::SetAutoSize method. Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize() in C++.'
type: docs
weight: 3000
url: /cpp/aspose.cells/comment/setautosize/
---
## Comment::SetAutoSize method


Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize().

```cpp
void Aspose::Cells::Comment::SetAutoSize(bool value)
```


## Examples


```cpp
if (!comment1.GetAutoSize())
{
    //The size of the comment varies with the content
    comment1.SetAutoSize(true);
}
```

## See Also

* Class [Vector](../../vector/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
