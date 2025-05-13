---
title: OleObject.ProgID
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets or sets the ProgID of the OLE object
type: docs
url: /net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Gets or sets the ProgID of the OLE object.

```csharp
public string ProgID { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(objOle.ProgID);
public void OleObject_Property_ProgID()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    int idxOle = 0;
    OleObject objOle = worksheet.OleObjects[idxOle];
    Console.WriteLine(objOle.ObjectData.ToString());
    Console.WriteLine(objOle.ProgID);
    Console.WriteLine(objOle.ObjectSourceFullName);
    Console.WriteLine(objOle.Label);
    Console.WriteLine(objOle.Text);
    Assert.AreEqual(FileFormatType.Pdf, objOle.FileFormatType);

    idxOle = 1;
    objOle = worksheet.OleObjects[idxOle];
    Console.WriteLine(objOle.ObjectData.ToString());
    Console.WriteLine(objOle.ProgID);
    Console.WriteLine(objOle.ObjectSourceFullName);
    Console.WriteLine(objOle.Label);
    Console.WriteLine(objOle.Text);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


