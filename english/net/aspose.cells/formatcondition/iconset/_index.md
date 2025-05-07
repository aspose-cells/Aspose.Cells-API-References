---
title: FormatCondition.IconSet
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings IconSet instance. The default instances IconSetType is TrafficLights31. Valid only for type  IconSet
type: docs
url: /net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(IconSetType.Arrows3, fcs[0].IconSet.Type);
[Test]
        public void Property_IconSet()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47217_iconset.ods");
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.IconSet);
            Assert.AreEqual(IconSetType.Arrows3, fcs[0].IconSet.Type);
            workbook.Save(Constants.destPath+ "CellsNet47217_iconset.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet47217_iconset.ods");
            fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.IconSet);
            Assert.AreEqual(IconSetType.Arrows3, fcs[0].IconSet.Type);
        }
```

### See Also

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


