---
title: Enum PresetShadowType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.PresetShadowType enum. Represents preset shadow type
type: docs
url: /net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Represents preset shadow type.

```csharp
public enum PresetShadowType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| NoShadow | `0` | No shadow. |
| Custom | `1` | Custom shadow. |
| OffsetDiagonalBottomRight | `2` | Outer shadow offset diagonal bottom right. |
| OffsetBottom | `3` | Outer shadow offset bottom. |
| OffsetDiagonalBottomLeft | `4` | Outer shadow offset diagonal bottom left. |
| OffsetRight | `5` | Outer shadow offset right. |
| OffsetCenter | `6` | Outer shadow offset center. |
| OffsetLeft | `7` | Outer shadow offset left. |
| OffsetDiagonalTopRight | `8` | Outer shadow offset diagonal top right. |
| OffsetTop | `9` | Outer shadow offset top. |
| OffsetDiagonalTopLeft | `10` | Outer shadow offset diagonal top left. |
| InsideDiagonalTopLeft | `11` | Inner shadow inside diagonal top Left. |
| InsideTop | `12` | Inner shadow inside top. |
| InsideDiagonalTopRight | `13` | Inner shadow inside diagonal top right. |
| InsideLeft | `14` | Inner shadow inside left. |
| InsideCenter | `15` | Inner shadow inside center. |
| InsideRight | `16` | Inner shadow inside right. |
| InsideDiagonalBottomLeft | `17` | Inner shadow inside diagonal bottom left. |
| InsideBottom | `18` | Inner shadow inside bottom. |
| InsideDiagonalBottomRight | `19` | Inner shadow inside diagonal bottom right. |
| PerspectiveDiagonalUpperLeft | `20` | Outer shadow perspective diagonal upper left. |
| PerspectiveDiagonalUpperRight | `21` | Outer shadow perspective diagonal upper right. |
| Below | `22` | Outer shadow below. |
| PerspectiveDiagonalLowerLeft | `23` | Outer shadow perspective diagonal lower left. |
| PerspectiveDiagonalLowerRight | `24` | Outer shadow perspective diagonal lower right. |

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Shapes[0].ShadowEffect.PresetType, PresetShadowType.NoShadow);
[Test]
        public void Type_PresetShadowType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET49239.xlsm&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET49239.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET49239.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Shapes[0].ShadowEffect.PresetType, PresetShadowType.NoShadow);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


