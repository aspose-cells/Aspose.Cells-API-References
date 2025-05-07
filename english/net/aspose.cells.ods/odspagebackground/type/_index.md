---
title: OdsPageBackground.Type
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the page background type
type: docs
url: /net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Gets and sets the page background type.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(b.Type ,OdsPageBackgroundType.Graphic);
[Test]
        public void Property_Type()
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

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


