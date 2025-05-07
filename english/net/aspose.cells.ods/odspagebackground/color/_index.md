---
title: OdsPageBackground.Color
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the color of background
type: docs
url: /net/aspose.cells.ods/odspagebackground/color/
---
## OdsPageBackground.Color property

Gets and sets the color of background.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(Color.Red, b.Color);
[Test]
        public void Property_Color()
        {
            Workbook workbook = new Workbook();
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            OdsPageBackground b = ps.ODSPageBackground;
            b.Type = OdsPageBackgroundType.Color;
            b.Color = Color.Red;
            workbook.Save(Constants.destPath + "CellsNet46695_2.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet46695_2.ods");
            ps = workbook.Worksheets[0].PageSetup;
            b = ps.ODSPageBackground;
            Assert.AreEqual(b.Type, OdsPageBackgroundType.Color);
           AssertHelper.AreEqual(Color.Red, b.Color);
        }
```

### See Also

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


