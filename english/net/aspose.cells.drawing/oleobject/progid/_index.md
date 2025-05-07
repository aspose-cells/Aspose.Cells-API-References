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
// Called: newEmbeddedObject.ProgID = "AcroExch.Document.DC";
[Test]
        public void Property_ProgID()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45834.Xls");
            workbook.Worksheets[0].OleObjects.RemoveAt(0);
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            //Add pdf
            byte[] iconData = File.ReadAllBytes(Constants.sourcePath + @"CellsNet45834.Emf");
            int newOleNumber = workbook.Worksheets[0].OleObjects.Add(10, 10, 533, 533, iconData);
            OleObject newEmbeddedObject = workbook.Worksheets[0].OleObjects[newOleNumber];
            newEmbeddedObject.ObjectData = File.ReadAllBytes(Constants.sourcePath + @"CellsNet45834.pdf");
            newEmbeddedObject.ProgID = "AcroExch.Document.DC";
            newEmbeddedObject.DisplayAsIcon = false;
            newEmbeddedObject.FileFormatType = (FileFormatType)13; // pdf format.
            Util.SaveManCheck(workbook, "Shape", "CellsNet45834.xls");
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


