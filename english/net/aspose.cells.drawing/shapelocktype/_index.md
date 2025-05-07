---
title: Enum ShapeLockType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapeLockType enum. Represents type of the property to be locked
type: docs
url: /net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Represents type of the property to be locked.

```csharp
public enum ShapeLockType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Group | `0` | Group |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Text |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |

### Examples

```csharp
// Called: Assert.IsFalse(ps.GetPicture(true, 0).GetLockedProperty(ShapeLockType.AspectRatio));
[Test]
        public void Type_ShapeLockType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet53788.xlsx");
            PageSetup ps = workbook.Worksheets[0].PageSetup;
           Assert.IsFalse(ps.GetPicture(true, 0).GetLockedProperty(ShapeLockType.AspectRatio));
            Assert.IsTrue(ps.GetPicture(false, 1).GetLockedProperty(ShapeLockType.AspectRatio));
            workbook.Save(Constants.destPath + "CellsNet53788.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


