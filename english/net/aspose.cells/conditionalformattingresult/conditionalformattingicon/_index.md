---
title: ConditionalFormattingResult.ConditionalFormattingIcon
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingResult property. Gets the image of icon set
type: docs
url: /net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Gets the image of icon set.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(IconSetType.TrafficLights31, res.ConditionalFormattingIcon.Type, "A1's IconSetType");
[Test]
        public void Property_ConditionalFormattingIcon()
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

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


