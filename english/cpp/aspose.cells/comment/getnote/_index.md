---
title: Aspose::Cells::Comment::GetNote method
linktitle: GetNote
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Comment::GetNote method. Represents the content of comment in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells/comment/getnote/
---
## Comment::GetNote method


Represents the content of comment.

```cpp
U16String Aspose::Cells::Comment::GetNote()
```

## Remarks


If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment. 

## Examples


```cpp
U16String note1 = comment1.GetNote();
U16String note2 = comment2.GetNote();
```

## See Also

* Class [U16String](../../u16string/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
