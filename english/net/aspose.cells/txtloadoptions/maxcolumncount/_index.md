---
title: TxtLoadOptions.MaxColumnCount
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. The maximum count of columns to be imported for one sheet
type: docs
url: /net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

The maximum count of columns to be imported for one sheet.

```csharp
public int MaxColumnCount { get; set; }
```

### Remarks

Those columns exceeding this limit will be ignored or extended to next sheet according to [`ExtendToNextSheet`](../extendtonextsheet/). This count includes the header columns([`HeaderColumnsCount`](../headercolumnscount/)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


