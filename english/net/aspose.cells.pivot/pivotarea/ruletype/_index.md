---
title: PivotArea.RuleType
second_title: Aspose.Cells for .NET API Reference
description: PivotArea property. Gets and sets the type of selection rule
type: docs
url: /net/aspose.cells.pivot/pivotarea/ruletype/
---
## PivotArea.RuleType property

Gets and sets the type of selection rule.

```csharp
public PivotAreaType RuleType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PivotAreaType.Button, pfc.PivotAreas[0].RuleType);
public void PivotArea_Property_RuleType()
{
    Workbook book = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");

    PivotTable pivot = book.Worksheets[0].PivotTables[0];
    // pivot.AddFieldToArea(PivotFieldType.Page, "year");
    pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

    //Add PivotFormatCondition
    int formatIndex = pivot.ConditionalFormats.Add();
    PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
    pfc.AddCellArea(CellArea.CreateCellArea("I12", "J12"));
    Assert.AreEqual(2, pfc.PivotAreas.Count);
    Assert.AreEqual(PivotAreaType.Button, pfc.PivotAreas[0].RuleType);
    Assert.AreEqual(PivotAreaType.Normal, pfc.PivotAreas[1].RuleType);
    FormatConditionCollection fcc = pfc.FormatConditions;



    int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
    FormatCondition fc = pfc.FormatConditions[index];
    fc.Formula1 = "100";
    fc.Operator = OperatorType.GreaterOrEqual;
    fc.Style.BackgroundColor = Color.Red;

    pivot.CalculateData();
    CellArea ca = fcc.GetCellArea(0);
    Assert.IsTrue(CellAreaTest.equals(ca, CellArea.CreateCellArea("I12", "J12"), "Area"));
    book.Save(Constants.PivotTableDestPath + "example.xlsx");

}
```

### See Also

* enum [PivotAreaType](../../pivotareatype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


