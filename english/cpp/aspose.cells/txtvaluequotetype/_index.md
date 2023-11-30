---
title: Aspose::Cells::TxtValueQuoteType enum
linktitle: TxtValueQuoteType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::TxtValueQuoteType enum. Specifies the type of using quotation marks for values in text format files in C++.'
type: docs
weight: 25900
url: /cpp/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enum


Specifies the type of using quotation marks for values in text format files.

```cpp
enum class TxtValueQuoteType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | 0 | All values that contain special characters such as quotation mark, separator character will be quoted. Same with the behavior of ms excel for exporting text file. |
| Always | 1 | All values will be quoted always. |
| Minimum | 2 | Only quote values when needed. Such as, if one value contains quotation mark but the quotation mark is not at the begin of this value, this value will not be quoted. |
| Never | 3 | All values will not be quoted. The exported text file with this type may not be read back correctly because the needed quotation marks being absent. |

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
