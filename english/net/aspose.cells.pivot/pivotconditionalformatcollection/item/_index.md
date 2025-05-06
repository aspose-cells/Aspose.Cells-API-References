---
title: PivotConditionalFormatCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormatCollection property. Gets the pivot FormatCondition object at the specific index
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformatcollection/item/
---
## PivotConditionalFormatCollection indexer

Gets the pivot FormatCondition object at the specific index.

```csharp
public PivotConditionalFormat this[int index] { get; }
```

### Return Value

pivot FormatCondition object.

### Examples

```csharp
// Called: PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
private void Property_Int32_(CellArea cellarea, PivotAreaType areaType )
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
            fc.Formula1 = &quot;100&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            pivot.CalculateData();
            Assert.IsTrue(CellAreaTest.equals(ca, cellarea, &quot;Area&quot;));

        }
```

### See Also

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


