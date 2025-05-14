---
title: Worksheet.OleObjects
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents a collection of OleObject in a worksheet
type: docs
url: /net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Represents a collection of [`OleObject`](../../../aspose.cells.drawing/oleobject/) in a worksheet.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Examples

```csharp
// Called: ole = workbook.Worksheets[0].OleObjects[1];
public void Worksheet_Property_OleObjects()
{
    string filePath = Constants.sourcePath + "example.xlsx";
    Workbook workbook = new Workbook(filePath);
    OleObject ole = workbook.Worksheets[0].OleObjects[1];
    string newName = ole.ObjectSourceFullName.Replace("Schatzkarte", "test");
    ole.ObjectSourceFullName = newName;
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    ole = workbook.Worksheets[0].OleObjects[1];
    Assert.AreEqual(ole.ObjectSourceFullName, newName);
}
```

### See Also

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


