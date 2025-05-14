---
title: StyleFlag.All
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. All properties will be applied
type: docs
url: /net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

All properties will be applied.

```csharp
public bool All { get; set; }
```

### Examples

```csharp
// Called: sf.All = true;
public void StyleFlag_Property_All()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 8].Value = "End";
    Column c = cells.Columns[1];
    Style s = wb.CreateStyle();
    s.Pattern = BackgroundType.Solid;
    s.ForegroundColor = Color.Red;
    StyleFlag sf = new StyleFlag();
    sf.All = true;
    c.ApplyStyle(s, sf);
    Aspose.Cells.Range r1 = cells.CreateRange(0, 0, 1, 3);
    Aspose.Cells.Range r2 = cells.CreateRange(0, 4, 1, 3);
    r2.Copy(r1);
    s = cells[0, 5].GetStyle();
    Assert.AreEqual(BackgroundType.Solid, s.Pattern, "Pattern");
    AssertHelper.AreEqual(Color.Red, s.ForegroundColor, "Color");
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


