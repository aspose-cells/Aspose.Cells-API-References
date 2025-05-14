---
title: OleObject.ObjectData
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Represents embedded ole object data as byte array
type: docs
url: /net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Represents embedded ole object data as byte array.

```csharp
public byte[] ObjectData { get; set; }
```

### Examples

```csharp
// Called: worksheet.OleObjects[oi].ObjectData = System.IO.File.ReadAllBytes(Constants.sourcePath + "test.xls");
public void OleObject_Property_ObjectData()
{
    var workbook = new Workbook();
    workbook.Worksheets[0].Name = "wksheet0";
    workbook.Worksheets.Add("wksheet1");

    for (var index = 0; index < 2; ++index)
    {
        var worksheet = workbook.Worksheets[index];
        var oi = worksheet.OleObjects.Add(1, 1, 600, 600, System.IO.File.ReadAllBytes(Constants.sourcePath + @"Image/logo.jpg"));
        worksheet.OleObjects[oi].ObjectData = System.IO.File.ReadAllBytes(Constants.sourcePath + "test.xls");
    }
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    for (var index = 0; index < 2; ++index)
    {
        var worksheet = workbook.Worksheets[index];
        var oi = worksheet.OleObjects.Add(1, 16, 600, 600, System.IO.File.ReadAllBytes(Constants.sourcePath + @"Image/logo.jpg"));
        worksheet.OleObjects[oi].ObjectData = System.IO.File.ReadAllBytes(Constants.sourcePath + "test.xls");
    }
    workbook.Worksheets.ActiveSheetIndex = 1;
    Util.SetHintMessage(workbook.Worksheets[1].Cells[0, 0], "Focus on the two OleObjects, they should not be changed to Picture.");
    Util.SaveManCheck(workbook, "Shape", "example.xlsx");
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook workbookSave = new Workbook();
    workbookSave.Copy(workbook);
    workbookSave.Worksheets.Add();
    workbookSave.Worksheets.Add();
    Util.SaveManCheck(workbook, "Shape", "example.xlsx");
}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


