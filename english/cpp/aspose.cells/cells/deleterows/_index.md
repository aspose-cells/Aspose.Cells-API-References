﻿---
title: Aspose::Cells::Cells::DeleteRows method
linktitle: DeleteRows
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Cells::DeleteRows method. Deletes several rows in C++.'
type: docs
weight: 11100
url: /cpp/aspose.cells/cells/deleterows/
---
## Cells::DeleteRows(int32_t, int32_t) method


Deletes several rows.

```cpp
bool Aspose::Cells::Cells::DeleteRows(int32_t rowIndex, int32_t totalRows)
```


| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int32_t | The first row index to be deleted. |
| totalRows | int32_t | Count of rows to be deleted. |
## Remarks



If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel. 
## See Also

* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::DeleteRows(int32_t, int32_t, bool) method


Deletes multiple rows in the worksheet.

```cpp
bool Aspose::Cells::Cells::DeleteRows(int32_t rowIndex, int32_t totalRows, bool updateReference)
```


| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | int32_t | Index of the first row to be deleted. |
| totalRows | int32_t | Count of rows to be deleted. |
| updateReference | bool | Indicates whether update references in other worksheets. |

## ReturnValue



## See Also

* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
