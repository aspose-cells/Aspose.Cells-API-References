---
title: PivotTable.ConditionalFormats
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the conditional formats of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/conditionalformats/
---
## PivotTable.ConditionalFormats property

Gets the conditional formats of the pivot table.

```csharp
public PivotConditionalFormatCollection ConditionalFormats { get; }
```

### Examples

```csharp
// Called: PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
[Test]
        public void Property_ConditionalFormats()
        {
            Workbook book = new Workbook();
            
            PivotTable pivot = CreateATable(book);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            //Add PivotFormatCondition
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            //int formatIndex = pivot.PivotFormatConditions.Add();
            //PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields[0]);
            FormatConditionCollection fcc = pfc.FormatConditions;
           CellArea ca = fcc.GetCellArea(0);
           Assert.IsTrue( CellAreaTest.equals(ca, CellArea.CreateCellArea(&quot;B14&quot;,&quot;D18&quot;),&quot;Area&quot;));
            
            int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[index];
            fc.Formula1 = &quot;100&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            book.Save(Constants.destPath + &quot;CellsNet57427_1.xlsx&quot;);

        }
```

### See Also

* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


