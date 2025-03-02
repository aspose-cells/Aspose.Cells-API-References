﻿---
title: Aspose::Cells::Drawing::SignatureLine::GetTitle method
linktitle: GetTitle
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::SignatureLine::GetTitle method. Gets or sets the title of singer in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells.drawing/signatureline/gettitle/
---
## SignatureLine::GetTitle method


Gets or sets the title of singer.

```cpp
U16String Aspose::Cells::Drawing::SignatureLine::GetTitle()
```


## Examples


```cpp
// Create signature line object
SignatureLine s4;
if (s4.GetTitle().IsNull() || s4.GetTitle().IsEmpty())
{
    s4.SetTitle(u"Development Lead");
}
```

## See Also

* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
