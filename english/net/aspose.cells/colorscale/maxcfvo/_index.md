---
title: ColorScale.MaxCfvo
second_title: Aspose.Cells for .NET API Reference
description: ColorScale property. Get or set this ColorScales max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it
type: docs
url: /net/aspose.cells/colorscale/maxcfvo/
---
## ColorScale.MaxCfvo property

Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Examples

```csharp
// Called: fc.ColorScale.MaxCfvo.IsGTE = true;
[Test]
        public void Property_MaxCfvo()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            int idx = ws.ConditionalFormattings.Add();

            FormatConditionCollection fcc = ws.ConditionalFormattings[idx];

            CellArea ca = CellArea.CreateCellArea("A1", "A5"); fcc.AddArea(ca);

            idx = fcc.AddCondition(FormatConditionType.ColorScale);

            FormatCondition fc = fcc[idx];
            fc.ColorScale.Is3ColorScale = false;
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Yellow;

            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Red;

            workbook.Save(Constants.destPath + "CELLSNET44168.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET44168.xlsx");
            fc = workbook.Worksheets[0].ConditionalFormattings[0][0];
            Assert.AreEqual(fc.ColorScale.Is3ColorScale, false);
        }
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


