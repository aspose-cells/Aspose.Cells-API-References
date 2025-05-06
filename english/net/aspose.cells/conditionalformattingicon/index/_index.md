---
title: ConditionalFormattingIcon.Index
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIcon property. Gets and sets the icons index in the icon set
type: docs
url: /net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Gets and sets the icon's index in the icon set.

```csharp
public int Index { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, res.ConditionalFormattingIcon.Index, &amp;quot;A3&amp;apos;s IconIndex&amp;quot;);
[Test]
        public void Property_Index()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[&quot;A1&quot;].PutValue(1);
            cells[&quot;A2&quot;].PutValue(&quot;#DIV/0!&quot;);
            cells[&quot;A3&quot;].PutValue(3);
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            ConditionalFormattingResult res = cells[&quot;A1&quot;].GetConditionalFormattingResult();
            Assert.AreEqual(IconSetType.TrafficLights31, res.ConditionalFormattingIcon.Type, &quot;A1&apos;s IconSetType&quot;);
            Assert.AreEqual(0, res.ConditionalFormattingIcon.Index, &quot;A1&apos;s IconIndex&quot;);
            res = cells[&quot;A3&quot;].GetConditionalFormattingResult();
            Assert.AreEqual(IconSetType.TrafficLights31, res.ConditionalFormattingIcon.Type, &quot;A3&apos;s IconSetType&quot;);
            Assert.AreEqual(2, res.ConditionalFormattingIcon.Index, &quot;A3&apos;s IconIndex&quot;);
            res = cells[&quot;A2&quot;].GetConditionalFormattingResult();
            Assert.IsTrue(res == null || res.ConditionalFormattingIcon == null, &quot;A2 should have no formatting&quot;);
        }
```

### See Also

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


