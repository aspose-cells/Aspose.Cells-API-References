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
// Called: int formatIndex = pivot.ConditionalFormats.Add();
public void PivotTable_Property_ConditionalFormats()
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
   Assert.IsTrue( CellAreaTest.equals(ca, CellArea.CreateCellArea("B14","D18"),"Area"));
            
    int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
    FormatCondition fc = pfc.FormatConditions[index];
    fc.Formula1 = "100";
    fc.Operator = OperatorType.GreaterOrEqual;
    fc.Style.BackgroundColor = Color.Red;
    book.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


