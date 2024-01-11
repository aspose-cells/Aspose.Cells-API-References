---
title: Cell.NumberCategoryType
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents the category type of this cells number formatting
type: docs
url: /net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Represents the category type of this cell's number formatting.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Remarks

When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is Number; When cell's value is 0 or not numeric value, the returned type is Text.

### See Also

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


