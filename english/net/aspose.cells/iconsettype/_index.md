---
title: Enum IconSetType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.IconSetType enum. Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable and the icon order is reversible
type: docs
url: /net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable, and the icon order is reversible.

```csharp
public enum IconSetType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Arrows3 | `0` | 3 arrows icon set. |
| ArrowsGray3 | `1` | 3 gray arrows icon set. |
| Flags3 | `2` | 3 flags icon set. |
| Signs3 | `3` | 3 signs icon set. |
| Symbols3 | `4` | 3 symbols icon set (circled). |
| Symbols32 | `5` | 3 Symbols icon set (uncircled). |
| TrafficLights31 | `6` | 3 traffic lights icon set (unrimmed). |
| TrafficLights32 | `7` | 3 traffic lights icon set with thick black border. |
| Arrows4 | `8` | 4 arrows icon set. |
| ArrowsGray4 | `9` | 4 gray arrows icon set. |
| Rating4 | `10` | 4 ratings icon set. |
| RedToBlack4 | `11` | 4 'red to black' icon set. |
| TrafficLights4 | `12` | 4 traffic lights icon set. |
| Arrows5 | `13` | 5 arrows icon set. |
| ArrowsGray5 | `14` | 5 gray arrows icon set. |
| Quarters5 | `15` | 5 quarters icon set. |
| Rating5 | `16` | 5 rating icon set. |
| Stars3 | `17` | 3 stars set |
| Boxes5 | `18` | 5 boxes set |
| Triangles3 | `19` | 3 triangles set |
| None | `20` | None |
| CustomSet | `21` | CustomSet. This element is read-only. |
| Smilies3 | `22` | 3 smilies. Only for .ods. |
| ColorSmilies3 | `23` | 3 color smilies. Only for .ods. |

### Examples

```csharp
// Called: Assert.AreEqual(IconSetType.TrafficLights31, res.ConditionalFormattingIcon.Type, "A3's IconSetType");
public void Cells_Type_IconSetType()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells["A1"].PutValue(1);
    cells["A2"].PutValue("#DIV/0!");
    cells["A3"].PutValue(3);
    ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
    FormatConditionCollection fcs = cfs[cfs.Add()];
    fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
    FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
    ConditionalFormattingResult res = cells["A1"].GetConditionalFormattingResult();
    Assert.AreEqual(IconSetType.TrafficLights31, res.ConditionalFormattingIcon.Type, "A1's IconSetType");
    Assert.AreEqual(0, res.ConditionalFormattingIcon.Index, "A1's IconIndex");
    res = cells["A3"].GetConditionalFormattingResult();
    Assert.AreEqual(IconSetType.TrafficLights31, res.ConditionalFormattingIcon.Type, "A3's IconSetType");
    Assert.AreEqual(2, res.ConditionalFormattingIcon.Index, "A3's IconIndex");
    res = cells["A2"].GetConditionalFormattingResult();
    Assert.IsTrue(res == null || res.ConditionalFormattingIcon == null, "A2 should have no formatting");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


