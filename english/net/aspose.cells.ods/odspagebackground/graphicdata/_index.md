---
title: OdsPageBackground.GraphicData
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the graphic data
type: docs
url: /net/aspose.cells.ods/odspagebackground/graphicdata/
---
## OdsPageBackground.GraphicData property

Gets and sets the graphic data.

```csharp
public byte[] GraphicData { get; set; }
```

### Examples

```csharp
// Called: b.GraphicData = File.ReadAllBytes(Constants.sourcePath + "image1.png");
[Test]
        public void Property_GraphicData()
        {
            Workbook workbook = new Workbook();
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            OdsPageBackground b = ps.ODSPageBackground;
            b.Type = OdsPageBackgroundType.Graphic;
            b.GraphicData = File.ReadAllBytes(Constants.sourcePath + "image1.png");
            b.GraphicType = OdsPageBackgroundGraphicType.Area;
            workbook.Save(Constants.destPath + "CellsNet46695_1.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet46695_1.ods");

            ps = workbook.Worksheets[0].PageSetup;
            b = ps.ODSPageBackground;
            Assert.AreEqual(b.Type ,OdsPageBackgroundType.Graphic);
            Assert.AreEqual(b.GraphicType, OdsPageBackgroundGraphicType.Area);

        }
```

### See Also

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


