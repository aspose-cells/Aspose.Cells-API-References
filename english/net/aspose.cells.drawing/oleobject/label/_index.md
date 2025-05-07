---
title: OleObject.Label
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets and sets the display label of the linked ole object
type: docs
url: /net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Gets and sets the display label of the linked ole object.

```csharp
public string Label { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(oleObject.Label, "label_nameです");
[Test]
        public void Property_Label()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42543.xlsx");
            OleObject oleObject = workbook.Worksheets[0].OleObjects[0];
            Assert.AreEqual(oleObject.Label, "label_nameです");
            workbook.Save(Constants.destPath + "CELLSJAVA42543.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42543.xlsx");
            oleObject = workbook.Worksheets[0].OleObjects[0];
            Assert.AreEqual(oleObject.Label, "label_nameです");
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


