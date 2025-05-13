---
title: Range.FirstRow
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the index of the first row of the range
type: docs
url: /net/aspose.cells/range/firstrow/
---
## Range.FirstRow property

Gets the index of the first row of the range.

```csharp
public int FirstRow { get; }
```

### Examples

```csharp
// Called: return _worksheet.Cells[range.FirstRow, range.FirstColumn];
private Cell Range_Property_FirstRow(Worksheet _worksheet, string address)
        {
            var range = _worksheet.Cells.CreateRange(address);
            return _worksheet.Cells[range.FirstRow, range.FirstColumn];
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


