---
title: Aspose::Cells::CellValueType enum
linktitle: CellValueType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CellValueType enum. Specifies a cell value type in C++.'
type: docs
weight: 18100
url: /cpp/aspose.cells/cellvaluetype/
---
## CellValueType enum


Specifies a cell value type.

```cpp
enum class CellValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| IsUnknown | 0 | [Cell](../cell/) value type is unknown. |
| IsNull | 1 | Blank cell. Corresponding value should be null. |
| IsNumeric | 2 | [Cell](../cell/) value is numeric. Corresponding value must be int or double. |
| IsDateTime | 4 | [Cell](../cell/) value is datetime. Corresponding value must be DateTime. |
| IsString | 8 | [Cell](../cell/) value is string. Corresponding value must be string. |
| IsBool | 16 | [Cell](../cell/) value is boolean. Corresponding value must be bool. |
| IsError | 32 | [Cell](../cell/) contains error value. Corresponding value must be error string. |

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
