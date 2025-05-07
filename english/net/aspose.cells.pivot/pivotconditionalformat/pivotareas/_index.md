---
title: PivotConditionalFormat.PivotAreas
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat property. Gets all pivot areas
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/pivotareas/
---
## PivotConditionalFormat.PivotAreas property

Gets all pivot areas.

```csharp
public PivotAreaCollection PivotAreas { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PivotAreaType.All, pfc.PivotAreas[0].RuleType);
[Test]
        public void Property_PivotAreas()
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
            book.Save(Constants.destPath + "CellsNet57465.xlsx");

        }
```

### See Also

* class [PivotAreaCollection](../../pivotareacollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


