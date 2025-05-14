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
private void PivotConditionalFormat_Property_FormatConditions(CellArea ca)
        {
            Workbook book = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");

            PivotTable pivot = book.Worksheets[0].PivotTables[0];
            //Add PivotFormatCondition
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(ca);

            FormatConditionCollection fcc = pfc.FormatConditions;

            //Aspose.Cells.Font font = null;
            //font.SchemeType = FontSchemeType.None;

            int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[index];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            pivot.CalculateData();
            CellArea r = fcc.GetCellArea(0);
            book.Save(Constants.destPath + "example.xlsx");
            Assert.IsTrue(CellAreaTest.equals(ca, r, "Area"));
        }
```

### See Also

* class [FormatConditionCollection](../../../aspose.cells/formatconditioncollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


