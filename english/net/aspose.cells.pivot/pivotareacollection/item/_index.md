---
title: PivotAreaCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotAreaCollection property. Gets a PivotArea object
type: docs
url: /net/aspose.cells.pivot/pivotareacollection/item/
---
## PivotAreaCollection indexer

Gets a [`PivotArea`](../../pivotarea/) object;

```csharp
public PivotArea this[int index] { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PivotAreaType.All, pfc.PivotAreas[0].RuleType);
public void PivotAreaCollection_Property_Item()
{
    Workbook book = new Workbook();

    PivotTable pivot = CreateATable(book);
    pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

    //Add PivotFormatCondition
    int formatIndex = pivot.ConditionalFormats.Add();
    PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
    pfc.AddCellArea(CellArea.CreateCellArea("A12","D18"));
    Assert.AreEqual(1,pfc.PivotAreas.Count);
    Assert.AreEqual(PivotAreaType.All, pfc.PivotAreas[0].RuleType);
    FormatConditionCollection fcc = pfc.FormatConditions;
    CellArea ca = fcc.GetCellArea(0);
          

    int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
    FormatCondition fc = pfc.FormatConditions[index];
    fc.Formula1 = "100";
    fc.Operator = OperatorType.GreaterOrEqual;
    fc.Style.BackgroundColor = Color.Red;
    pivot.CalculateData();
    Assert.IsTrue(CellAreaTest.equals(ca, CellArea.CreateCellArea("A12", "D18"), "Area"));
    book.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


