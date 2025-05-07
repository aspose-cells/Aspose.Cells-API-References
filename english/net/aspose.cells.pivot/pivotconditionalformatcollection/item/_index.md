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
private void Property_Int32_(string file,CellArea ca)
        {
            Workbook book = new Workbook(file);

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
            book.Save(Constants.destPath + "CellsNet57571.xlsx");
            Assert.IsTrue(CellAreaTest.equals(ca, r, "Area"));
        }
```

### See Also

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


