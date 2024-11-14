---
title: Aspose::Cells::Drawing::SignatureLine::GetEmail method
linktitle: GetEmail
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::SignatureLine::GetEmail method. Gets or sets the email of singer in C++.'
type: docs
weight: 1400
url: /cpp/aspose.cells.drawing/signatureline/getemail/
---
## SignatureLine::GetEmail method


Gets or sets the email of singer.

```cpp
U16String Aspose::Cells::Drawing::SignatureLine::GetEmail()
```


## Examples


```cpp
// Create signature line object
SignatureLine s5;
if (s5.GetEmail().IsNull() || s5.GetEmail().IsEmpty())
{
    s5.SetEmail(u"Simon.Zhao@aspose.com");
}
```

## See Also

* Class [U16String](../../../aspose.cells/u16string/)
* Class [SignatureLine](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
