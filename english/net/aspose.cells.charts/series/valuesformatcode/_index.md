---
title: Series.ValuesFormatCode
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents format code of Valuess NumberList
type: docs
url: /net/aspose.cells.charts/series/valuesformatcode/
---
## Series.ValuesFormatCode property

Represents format code of Values's NumberList.

```csharp
public string ValuesFormatCode { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("0.00%",chart.NSeries[0].ValuesFormatCode);
public void Series_Property_ValuesFormatCode()
{
    string filePath = Constants.PivotTableSourcePath + @"NET44443_";
    Workbook wb = new Workbook(filePath + "test.xlsx");
    //wb.Worksheets["Test"].Charts[0].RefreshPivotData();
    //wb.Save(CreateFolder(filePath) + "out.pdf");

    wb.Worksheets.RefreshAll();
    Chart chart1 = wb.Worksheets["Test"].Charts[0];
    Assert.AreEqual("=Sheet1!$C$4:$C$13", chart1.NSeries[0].Values);
    Chart chart = wb.Worksheets["Sheet1"].Charts[0];
   Assert.AreEqual("0.00%",chart.NSeries[0].ValuesFormatCode);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


