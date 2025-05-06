---
title: PivotConditionalFormat.FormatConditions
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat property. Get conditions for the pivot table conditional format 
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/formatconditions/
---
## PivotConditionalFormat.FormatConditions property

Get conditions for the pivot table conditional format .

```csharp
public FormatConditionCollection FormatConditions { get; }
```

### Examples

```csharp
// Called: FormatCondition fc = pfc.FormatConditions[index];
[Test]
        public void Property_FormatConditions()
        {
            Workbook book = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet57464.xlsx&quot;);

            PivotTable pivot = book.Worksheets[0].PivotTables[0];
            // pivot.AddFieldToArea(PivotFieldType.Page, &quot;year&quot;);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            //Add PivotFormatCondition
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea(&quot;I12&quot;, &quot;J12&quot;));
            Assert.AreEqual(2, pfc.PivotAreas.Count);
            Assert.AreEqual(PivotAreaType.Button, pfc.PivotAreas[0].RuleType);
            Assert.AreEqual(PivotAreaType.Normal, pfc.PivotAreas[1].RuleType);
            FormatConditionCollection fcc = pfc.FormatConditions;



            int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[index];
            fc.Formula1 = &quot;100&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            pivot.CalculateData();
            CellArea ca = fcc.GetCellArea(0);
            Assert.IsTrue(CellAreaTest.equals(ca, CellArea.CreateCellArea(&quot;I12&quot;, &quot;J12&quot;), &quot;Area&quot;));
            book.Save(Constants.PivotTableDestPath + &quot;CellsNet57464.xlsx&quot;);

        }
```

### See Also

* class [FormatConditionCollection](../../../aspose.cells/formatconditioncollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


