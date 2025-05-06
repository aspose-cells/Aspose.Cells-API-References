---
title: PivotField.ShowValuesAs
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Shows values of data field as different display format when the ShowDataAs calculation is in use
type: docs
url: /net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## PivotField.ShowValuesAs method

Shows values of data field as different display format when the ShowDataAs calculation is in use.

```csharp
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | The data display format type. |
| baseField | Int32 | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | PivotItemPositionType | The position type of base iteam. |
| baseItem | Int32 | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |

### Remarks

Only for data field.

### Examples

```csharp
// Called: pfDiff.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, pfBase.BaseIndex, PivotItemPositionType.Next,0);
[Test]
        public void Method_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43358_&quot;;

            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = &quot;Sheet&quot;;
            ws.Cells[0, 0].PutValue(&quot;X&quot;);
            ws.Cells[0, 1].PutValue(&quot;Y&quot;);
            ws.Cells[0, 2].PutValue(&quot;Data&quot;);
            ws.Cells[0, 3].PutValue(&quot;Data2&quot;);

            ws.Cells[1, 0].PutValue(&quot;A&quot;);
            ws.Cells[1, 1].PutValue(&quot;C&quot;);
            ws.Cells[1, 2].PutValue(10);
            ws.Cells[1, 3].PutValue(122);

            ws.Cells[2, 0].PutValue(&quot;A&quot;);
            ws.Cells[2, 1].PutValue(&quot;D&quot;);
            ws.Cells[2, 2].PutValue(25);
            ws.Cells[2, 3].PutValue(23);

            ws.Cells[3, 0].PutValue(&quot;B&quot;);
            ws.Cells[3, 1].PutValue(&quot;C&quot;);
            ws.Cells[3, 2].PutValue(30);
            ws.Cells[3, 3].PutValue(22);

            ws.Cells[4, 0].PutValue(&quot;B&quot;);
            ws.Cells[4, 1].PutValue(&quot;D&quot;);
            ws.Cells[4, 2].PutValue(45);
            ws.Cells[4, 3].PutValue(78);



            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add(&quot;=Sheet!A1:D5&quot;, &quot;A7&quot;, &quot;PivotTable1&quot;);
            PivotTable pt = ptc[index];

            int fp;
            PivotField pf;
            PivotField pfBase;

            fp = pt.AddFieldToArea(PivotFieldType.Row, &quot;X&quot;);
            pf = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, &quot;Y&quot;);
            pfBase = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, &quot;Data&quot;);
            pf = pt.Fields(PivotFieldType.Data)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, &quot;Data2&quot;);
            pf = pt.Fields(PivotFieldType.Data)[fp];


            int fieldPosition = pt.AddFieldToArea(PivotFieldType.Data, &quot;Data&quot;);
            PivotField pfDiff = pt.Fields(PivotFieldType.Data)[fieldPosition];
            pfDiff.DisplayName = &quot;Diff&quot;;
            pfDiff.Function = ConsolidationFunction.Sum;
            pfDiff.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, pfBase.BaseIndex, PivotItemPositionType.Next,0);
            //pfDiff.DataDisplayFormat = PivotFieldDataDisplayFormat.DifferenceFrom;

            ////构造时 未指定类型，所以写出时要分别对待 
            //pfDiff.BaseItemPosition = PivotItemPosition.Next; //Commenting out this line produces valid file 
            //pfDiff.BaseFieldIndex = pfBase.BaseIndex;


            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);

            wb.CalculateFormula();
            wb.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET43358.xls&quot;);
            wb.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET43358.xlsx&quot;);
        }
```

### See Also

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


