---
title: Worksheet.Protection
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version
type: docs
url: /net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version.

```csharp
public Protection Protection { get; }
```

### Remarks

This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.

### Examples

```csharp
// Called: Assert.IsFalse(sheet.Protection.AllowEditingObject);
public void Worksheet_Property_Protection()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml");
    Worksheet sheet = workbook.Worksheets[0];
    Assert.IsFalse(sheet.Protection.AllowEditingScenario);
    Assert.IsFalse(sheet.Protection.AllowEditingObject);
    workbook.Save(Constants.destPath + "example.xml");
    workbook = new Workbook(Constants.destPath + "example.xml");
    Assert.IsFalse(sheet.Protection.AllowEditingScenario);
    Assert.IsFalse(sheet.Protection.AllowEditingObject);
    workbook.Save(Constants.destPath + "example.xml");
}
```

### See Also

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


