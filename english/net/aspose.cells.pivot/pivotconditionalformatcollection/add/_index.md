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
[Test]
        public void Method_Add()
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
            book.Save(Constants.destPath + "CellsNet57427_1.xlsx");

        }
```

### See Also

* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


