---
title: TxtLoadOptions.MaxRowCount
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. The maximum count of rows to be imported for one sheet
type: docs
url: /net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

The maximum count of rows to be imported for one sheet.

```csharp
public int MaxRowCount { get; set; }
```

### Remarks

Those rows exceeding this limit will be ignored or extended to next sheet according to [`ExtendToNextSheet`](../extendtonextsheet/). This count includes the header rows([`HeaderRowsCount`](../headerrowscount/)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


