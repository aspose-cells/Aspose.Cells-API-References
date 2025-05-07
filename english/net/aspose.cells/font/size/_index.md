---
title: Font.Size
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the size of the font
type: docs
url: /net/aspose.cells/font/size/
---
## Font.Size property

Gets or sets the size of the font.

```csharp
public int Size { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(20, style.Font.Size);
[Test]
        public void Property_Size()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA-41541.xml");
            Assert.AreEqual(10, workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Size);
         
            workbook.Save(Constants.destPath + "dest.xlsx");
             workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41541_1.xml");
            Assert.AreEqual(10, workbook.Worksheets[0].Cells["A7"].GetStyle().Font.Size);
            Style style = workbook.Worksheets[1].Cells["A1"].GetStyle();
            Assert.AreEqual(20, style.Font.Size);
            Assert.AreEqual("base format s31", style.ParentStyle.Name);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


