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
// Called: var o = wb.Worksheets[0].OleObjects[0];
[Test]
        public void Property_OleObjects()
        {

            string filePath = Constants.sourcePath + &quot;CellsNet45226.xlsx&quot;;
            var asposeOptions = new Aspose.Cells.LoadOptions { MemorySetting = MemorySetting.MemoryPreference };
            var wb = new Workbook(filePath, asposeOptions);
            //var o = wb.Worksheets[0].Shapes[0] as OleObject; //also does not worth 
            var o = wb.Worksheets[0].OleObjects[0];

            var updatedPath = @&quot;c:\temp\Images\test.bmp&quot;;
            o.ObjectSourceFullName = updatedPath;
            o.UpdateSelectedValue();
            wb.Save(Constants.destPath + &quot;CellsNet45226.xlsx&quot;);
            Workbook workbook = new Workbook(Constants.destPath + &quot;CellsNet45226.xlsx&quot;);
            OleObject ole = wb.Worksheets[0].OleObjects[0];
            Assert.AreEqual(ole.ObjectSourceFullName, updatedPath);

        }
```

### See Also

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


