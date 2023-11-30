---
title: Aspose::Cells::Drawing::SignatureLine::GetInstructions method
linktitle: GetInstructions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::SignatureLine::GetInstructions method. Gets and sets the text shown to user at signing time in C++.'
type: docs
weight: 1800
url: /cpp/aspose.cells.drawing/signatureline/getinstructions/
---
## SignatureLine::GetInstructions method


Gets and sets the text shown to user at signing time.

```cpp
U16String Aspose::Cells::Drawing::SignatureLine::GetInstructions()
```


## Examples


```cpp
    // Create signature line object
SignatureLine s6;
if (s6.GetInstructions().IsNull() || s6.GetInstructions().IsEmpty())
{
    s6.SetInstructions(u"Just do it.");
}
```

## See Also

* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
