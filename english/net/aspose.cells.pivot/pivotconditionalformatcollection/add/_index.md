---
title: PivotConditionalFormatCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormatCollection method. Adds a pivot FormatCondition to the collection
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformatcollection/add/
---
## PivotConditionalFormatCollection.Add method

Adds a pivot FormatCondition to the collection.

```csharp
public int Add()
```

### Return Value

pivot FormatCondition object index.

### Remarks

not supported

### Examples

```csharp
// Called: int formatIndex = pivot.ConditionalFormats.Add();
private void Method_Add(string file,CellArea ca)
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
            fc.Formula1 = &quot;100&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            pivot.CalculateData();
            CellArea r = fcc.GetCellArea(0);
            book.Save(Constants.destPath + &quot;CellsNet57571.xlsx&quot;);
            Assert.IsTrue(CellAreaTest.equals(ca, r, &quot;Area&quot;));
        }
```

### See Also

* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


