---
title: Enum RenameStrategy
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.RenameStrategy enum. Strategy option for duplicate names of columns
type: docs
url: /net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Strategy option for duplicate names of columns.

```csharp
public enum RenameStrategy
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Exception | `0` | Throws exception. |
| Digit | `1` | Named with digit. Duplicated names will become ...1, ...2, etc. |
| Letter | `2` | Named with letter.. Duplicated names will become ...A, ...B, etc. |

### Remarks

When processing data with headers, some scenarios require the headers to be no duplication for all columns. For example, when exporting data to a datatable and the header is required to be taken as datatable's column name, duplicated values of the header are invalid. For such kind of situations, user may determine how to handle them by specifying this strategy.

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


