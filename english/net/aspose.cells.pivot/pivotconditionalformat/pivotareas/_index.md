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
// Called: Assert.AreEqual(areaType, pfc.PivotAreas[0].RuleType);
private void PivotConditionalFormat_Property_PivotAreas(CellArea cellarea, PivotAreaType areaType )
        {
            Workbook book = new Workbook();

            PivotTable pivot = CreateATable(book);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            //Add PivotFormatCondition
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(cellarea);
            Assert.AreEqual(1, pfc.PivotAreas.Count);
            Assert.AreEqual(areaType, pfc.PivotAreas[0].RuleType);
            FormatConditionCollection fcc = pfc.FormatConditions;
            CellArea ca = fcc.GetCellArea(0);


            int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[index];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            pivot.CalculateData();
            Assert.IsTrue(CellAreaTest.equals(ca, cellarea, "Area"));

        }
```

### See Also

* class [PivotAreaCollection](../../pivotareacollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


