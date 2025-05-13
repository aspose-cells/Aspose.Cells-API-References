---
title: PageSetup.ODSPageBackground
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Gets the background of ODS
type: docs
url: /net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Gets the background of ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Examples

```csharp
// Called: OdsPageBackground b = ps.ODSPageBackground;
public void PageSetup_Property_ODSPageBackground()
{
    Workbook workbook = new Workbook();
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    OdsPageBackground b = ps.ODSPageBackground;
    b.Type = OdsPageBackgroundType.Color;
    b.Color = Color.Red;
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    ps = workbook.Worksheets[0].PageSetup;
    b = ps.ODSPageBackground;
    Assert.AreEqual(b.Type, OdsPageBackgroundType.Color);
   AssertHelper.AreEqual(Color.Red, b.Color);
}
```

### See Also

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


