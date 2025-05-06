---
title: ConditionalFormattingResult.ConditionalStyle
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingResult property. Gets the conditional result style
type: docs
url: /net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

Gets the conditional result style.

```csharp
public Style ConditionalStyle { get; }
```

### Examples

```csharp
// Called: Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
[Test]
        public void Property_ConditionalStyle()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/CellsNet42577.xlsx&quot;);
            Cell cell = wb.Worksheets[&quot;SB_01_G_DIT_00&quot;].Cells[&quot;G100&quot;];
            Style conditionalStyle = cell.GetConditionalFormattingResult().ConditionalStyle;
            Style cellStyle = cell.GetDisplayStyle();
            Assert.AreEqual(0x92D050, conditionalStyle.Font.Color.ToArgb()&amp;0xFFFFFF, &quot;ConditionalStyle.Font.Color&quot;);
            Assert.AreEqual(0x92D050, cellStyle.Font.Color.ToArgb() &amp; 0xFFFFFF, &quot;CellDisplayStyle.Font.Color&quot;);
            Assert.AreEqual(TextAlignmentType.Center, cellStyle.HorizontalAlignment, &quot;CellDisplayStyle.HorizontalAlignment&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


