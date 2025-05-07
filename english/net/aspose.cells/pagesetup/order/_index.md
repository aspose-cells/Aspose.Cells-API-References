---
title: PageSetup.Order
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the order that Microsoft Excel uses to number pages when printing a large worksheet
type: docs
url: /net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.

```csharp
public PrintOrderType Order { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(PrintOrderType.OverThenDown, sheet.PageSetup.Order, "sheet.PageSetup.Order");
private void Property_Order(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            AssertHelper.AreEqual(PrintOrderType.OverThenDown, sheet.PageSetup.Order, "sheet.PageSetup.Order");
        }
```

### See Also

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


