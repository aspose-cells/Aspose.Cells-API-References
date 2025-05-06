---
title: IconSet.Type
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get or Set the icon set type to display. Setting the type will auto check if the current Cfvoss count is accord with the new type. If not accord old Cfvos will be cleaned and default Cfvos will be added
type: docs
url: /net/aspose.cells/iconset/type/
---
## IconSet.Type property

Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.

```csharp
public IconSetType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(IconSetType.Arrows3, fcs[0].IconSet.Type);
[Test]
        public void Property_Type()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47217_iconset.ods&quot;);
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.IconSet);
            Assert.AreEqual(IconSetType.Arrows3, fcs[0].IconSet.Type);
            workbook.Save(Constants.destPath+ &quot;CellsNet47217_iconset.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet47217_iconset.ods&quot;);
            fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.IconSet);
            Assert.AreEqual(IconSetType.Arrows3, fcs[0].IconSet.Type);
        }
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


