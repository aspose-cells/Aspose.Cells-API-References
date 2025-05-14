---
title: PivotConditionalFormat.AddCellArea
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat method. Adds an area based on pivot table view
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/addcellarea/
---
## PivotConditionalFormat.AddCellArea method

Adds an area based on pivot table view.

```csharp
public void AddCellArea(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The cell area. |

### Examples

```csharp
// Called: pfc.AddCellArea(ca);
public void PivotConditionalFormat_Method_AddCellArea(CellArea ca )
        {
            Workbook book = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");

            PivotTable pivot = book.Worksheets[0].PivotTables[0];
            // pivot.AddFieldToArea(PivotFieldType.Page, "year");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

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
            Assert.IsTrue(CellAreaTest.equals(ca, r, "Area"));
           

        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


