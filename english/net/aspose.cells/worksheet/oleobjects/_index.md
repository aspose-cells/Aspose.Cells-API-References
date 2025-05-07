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
// Called: foreach (OleObject o in sheet.OleObjects)
[Test]
        public void Property_OleObjects()
        {

            Workbook d = new Workbook(Constants.sourcePath + "CELLSNET55768.xlsx");
            foreach (Worksheet sheet in d.Worksheets)
            {
                foreach (OleObject o in sheet.OleObjects)
                {
                   Assert.AreEqual(FileFormatType.Bmp, o.FileFormatType);
                   Assert.IsTrue(string.IsNullOrEmpty(o.ObjectSourceFullName));
                }
            }
        }
```

### See Also

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


