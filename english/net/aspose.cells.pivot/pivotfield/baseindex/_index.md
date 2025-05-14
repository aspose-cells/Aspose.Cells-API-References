---
title: PivotField.BaseIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the PivotField index in the base PivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfield/baseindex/
---
## PivotField.BaseIndex property

Represents the PivotField index in the base PivotFields.

```csharp
public int BaseIndex { get; set; }
```

### Examples

```csharp
// Called: pfDiff.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, pfBase.BaseIndex, PivotItemPositionType.Next,0);
public void PivotField_Property_BaseIndex()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43358_";

    Workbook wb = new Workbook();
    Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
    ws.Name = "Sheet";
    ws.Cells[0, 0].PutValue("X");
    ws.Cells[0, 1].PutValue("Y");
    ws.Cells[0, 2].PutValue("Data");
    ws.Cells[0, 3].PutValue("Data2");

    ws.Cells[1, 0].PutValue("A");
    ws.Cells[1, 1].PutValue("C");
    ws.Cells[1, 2].PutValue(10);
    ws.Cells[1, 3].PutValue(122);

    ws.Cells[2, 0].PutValue("A");
    ws.Cells[2, 1].PutValue("D");
    ws.Cells[2, 2].PutValue(25);
    ws.Cells[2, 3].PutValue(23);

    ws.Cells[3, 0].PutValue("B");
    ws.Cells[3, 1].PutValue("C");
    ws.Cells[3, 2].PutValue(30);
    ws.Cells[3, 3].PutValue(22);

    ws.Cells[4, 0].PutValue("B");
    ws.Cells[4, 1].PutValue("D");
    ws.Cells[4, 2].PutValue(45);
    ws.Cells[4, 3].PutValue(78);



    PivotTableCollection ptc = ws.PivotTables;
    int index = ptc.Add("=Sheet!A1:D5", "A7", "PivotTable1");
    PivotTable pt = ptc[index];

    int fp;
    PivotField pf;
    PivotField pfBase;

    fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
    pf = pt.Fields(PivotFieldType.Row)[fp];

    fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
    pfBase = pt.Fields(PivotFieldType.Column)[fp];

    fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
    pf = pt.Fields(PivotFieldType.Data)[fp];

    fp = pt.AddFieldToArea(PivotFieldType.Data, "Data2");
    pf = pt.Fields(PivotFieldType.Data)[fp];


    int fieldPosition = pt.AddFieldToArea(PivotFieldType.Data, "Data");
    PivotField pfDiff = pt.Fields(PivotFieldType.Data)[fieldPosition];
    pfDiff.DisplayName = "Diff";
    pfDiff.Function = ConsolidationFunction.Sum;
    pfDiff.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, pfBase.BaseIndex, PivotItemPositionType.Next,0);
    //pfDiff.DataDisplayFormat = PivotFieldDataDisplayFormat.DifferenceFrom;

    ////构造时 未指定类型，所以写出时要分别对待 
    //pfDiff.BaseItemPosition = PivotItemPosition.Next; //Commenting out this line produces valid file 
    //pfDiff.BaseFieldIndex = pfBase.BaseIndex;


    pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);

    wb.CalculateFormula();
    wb.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xls");
    wb.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


