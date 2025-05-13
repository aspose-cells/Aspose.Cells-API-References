---
title: Enum TextureType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.TextureType enum. Represents the preset texture type
type: docs
url: /net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Represents the preset texture type.

```csharp
public enum TextureType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| BlueTissuePaper | `0` | Represents Blue Tissue Paper texture type. |
| Bouquet | `1` | Represents Bouquet texture type. |
| BrownMarble | `2` | Represents Brown Marble texture type. |
| Canvas | `3` | Represents Canvas texture type. |
| Cork | `4` | Represents Cork texture type. |
| Denim | `5` | Represents Denim texture type. |
| FishFossil | `6` | Represents Fish Fossil texture type. |
| Granite | `7` | Represents Granite texture type. |
| GreenMarble | `8` | Represents Green Marble texture type. |
| MediumWood | `9` | Represents Medium Wood texture type. |
| Newsprint | `10` | Represents Newsprint texture type. |
| Oak | `11` | Represents Oak texture type. |
| PaperBag | `12` | Represents Paper Bag texture type. |
| Papyrus | `13` | Represents Papyrus texture type. |
| Parchment | `14` | Represents Parchment texture type. |
| PinkTissuePaper | `15` | Represents Pink Tissue Paper texture type. |
| PurpleMesh | `16` | Represents Purple Mesh texture type. |
| RecycledPaper | `17` | Represents Recycled Paper texture type. |
| Sand | `18` | Represents Sand texture type. |
| Stationery | `19` | Represents Stationery texture type. |
| Walnut | `20` | Represents Walnut Droplets texture type. |
| WaterDroplets | `21` | Represents Water Droplets texture type. |
| WhiteMarble | `22` | Represents White Marble texture type. |
| WovenMat | `23` | Represents Woven Mat texture type. |
| Unknown | `24` | Represents Unknown texture type. |

### Examples

```csharp
// Called: AssertHelper.AreEqual(TextureType.Stationery, p.Area.FillFormat.Texture, "chart.NSeries[3].Area.FillFormat.Texture");
private void Drawing_Type_TextureType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet1"];
            Chart chart = sheet.Charts[0];
            //Series aseries = chart.NSeries[3];
            ChartPoint p = chart.NSeries[0].Points[3];
            AssertHelper.AreEqual(TextureType.Stationery, p.Area.FillFormat.Texture, "chart.NSeries[3].Area.FillFormat.Texture");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


