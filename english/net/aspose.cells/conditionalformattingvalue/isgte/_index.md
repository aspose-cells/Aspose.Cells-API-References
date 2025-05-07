---
title: ConditionalFormattingValue.IsGTE
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValue property. Get or set the Greater Than Or Equal flag. Use only for icon sets determines whether this threshold value uses the greater than or equal to operator. false indicates greater than is used instead of greater than or equal to. Default value is true
type: docs
url: /net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

```csharp
public bool IsGTE { get; set; }
```

### Examples

```csharp
// Called: fc.ColorScale.MinCfvo.IsGTE = true;
[Test]
        public void Property_IsGTE()
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

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


