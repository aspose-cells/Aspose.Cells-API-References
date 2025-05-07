---
title: IconSet.IsCustom
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Indicates whether the icon set is custom. Default value is false
type: docs
url: /net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Indicates whether the icon set is custom. Default value is false.

```csharp
public bool IsCustom { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(fcs[0].IconSet.IsCustom);
[Test]
        public void Property_IsCustom()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CustomIconSet01.xlsx");
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.IconSet);
            Assert.IsTrue(fcs[0].IconSet.IsCustom);
            Assert.IsFalse(fcs[0].StopIfTrue);
        }
```

### See Also

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


