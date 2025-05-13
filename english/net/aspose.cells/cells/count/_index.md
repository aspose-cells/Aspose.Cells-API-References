---
title: Cells.Count
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the total count of instantiated Cell objects
type: docs
url: /net/aspose.cells/cells/count/
---
## Cells.Count property

Gets the total count of instantiated Cell objects.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(cells.Count > 0, "Cells should not be empty after save with ClearData=false");
public void Cells_Property_Count()
{
    string file = Constants.bugFilePath + "savetest.xls";
    Workbook workbook = new Workbook(file);
    XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
    saveOptions.ClearData = false;
    Util.SaveAsBuffer(workbook, saveOptions);
    Worksheet sheet = workbook.Worksheets[0];
    Cells cells = sheet.Cells;
    Assert.AreEqual(1, sheet.Shapes.Count);
    Assert.IsTrue(cells.Count > 0, "Cells should not be empty after save with ClearData=false");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


