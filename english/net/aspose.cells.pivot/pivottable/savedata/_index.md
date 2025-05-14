---
title: PivotTable.SaveData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether data for the PivotTable report is saved with the workbook
type: docs
url: /net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

Indicates whether data for the PivotTable report is saved with the workbook.

```csharp
public bool SaveData { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[1].PivotTables[0].SaveData = false;
public void PivotTable_Property_SaveData()
{

    Workbook workbook = new Workbook(Constants.openPivottablePath + "Test_PivotChartConnLost(1).xlsx");//source sheet
    workbook.Save(Constants.savePivottablePath + "testchart.xlsx");

    workbook = new Workbook(Constants.openPivottablePath + "test2(2).xls");//source sheet
    workbook.Worksheets[1].PivotTables[0].RefreshData();
    workbook.Worksheets[1].PivotTables[0].CalculateData();
    workbook.Save(Constants.savePivottablePath + "tt.xls");

    workbook = new Workbook(Constants.openPivottablePath + "test3.xls");//source sheet
    workbook.Worksheets[1].PivotTables[0].RefreshData();
    workbook.Worksheets[1].PivotTables[0].CalculateData();
    workbook.Save(Constants.savePivottablePath + "tt2.xls");

    //workbook = new Workbook("D:\\mmm.xls");//source sheet
    //workbook.Worksheets[0].PivotTables[0].RefreshData();
    //workbook.Worksheets[0].PivotTables[0].CalculateData();
    //workbook.Save("D:\\book_out.xls");

    workbook = new Workbook(Constants.openXlsbPath + "Copy of ExcelSource.xlsb");//source sheet
    workbook.Save(Constants.saveXlsbPath + "book_out.xlsb");

    workbook = new Workbook(Constants.openXlsbPath + "Excel Binary WorkBook.xlsb");//source sheet
    workbook.Save(Constants.saveXlsbPath + "Excel Binary WorkBook.xlsb");

    //www.aspose.com/community/forums/page_2/312315/showthread.aspx
    workbook = new Workbook(Constants.openXlsbPath + "ExcelSource2.xlsb");//source sheet
    workbook.Save(Constants.saveXlsbPath + "ExcelSource2.xlsb");

    workbook = new Workbook(Constants.openXlsbPath + "Book1.xlsm");//source sheet
    workbook.Save(Constants.saveXlsbPath + "book_1.xlsb");

    //www.aspose.com/community/forums/thread/296348.aspx
    workbook = new Workbook(Constants.openPivottablePath + "MasterTemplate.xltm");//source sheet
    workbook.Save(Constants.savePivottablePath + "MasterTemplate.xltm");

            

    /////www.aspose.com/community/forums/thread/296383.aspx
    workbook = new Workbook(Constants.openPivottablePath + "example.xlsx");//source sheet
    workbook.Worksheets[1].PivotTables[0].RefreshDataOnOpeningFile = true;
    //workbook.Worksheets[1].PivotTables[0].BaseFields[0].DataDisplayFormat = PivotFieldDataDisplayFormat.
    workbook.Worksheets[2].Cells["B4"].Value = 5;
    workbook.Worksheets[1].PivotTables[0].RefreshData();
    workbook.Worksheets[1].PivotTables[0].CalculateRange();
    //Assert.AreEqual(workbook.Worksheets[1].PivotTables[0].DataBodyRange.EndRow, 9);
    workbook.Save(Constants.savePivottablePath + "example.xlsx");

    //www.aspose.com/community/forums/page_2/297203/showthread.aspx
    workbook = new Workbook(Constants.openXlsbPath + "Resource Plan Template - Full v8.0.xlsm");//source sheet
    workbook.Save(Constants.saveXlsbPath + "Resource Plan Template - Full v8.0.xlsb");

    workbook = new Workbook(Constants.openXlsbPath + "kk.xlsx");//source sheet
    workbook.Save(Constants.saveXlsbPath + "kk.xlsb");
    workbook = new Workbook(Constants.openXlsbPath + "kk.xlsb");//source sheet
    //Assert.AreEqual(workbook.Worksheets[0].Cells[0].DoubleValue, 0);


    //www.aspose.com/community/forums/thread/302501/pivottables-choose-pivottable-options-data-and-un-check-save-source-data-with-file.aspx
    workbook = new Workbook(Constants.openPivottablePath + "mmm.xlsx");//source sheet
    workbook.Worksheets[1].PivotTables[0].SaveData = false;
    workbook.Save(Constants.savePivottablePath + "testmmm.xlsx");

    //www.aspose.com/community/forums/thread/303991.aspx
    workbook = new Workbook(Constants.openPivottablePath + "mmm.xlsx");//source sheet
    workbook.Worksheets[1].PivotTables[0].ShowDrill = false;
    workbook.Save(Constants.savePivottablePath + "example.xlsx");

    workbook = new Workbook(Constants.openPivottablePath + "Template.xlsx");//source sheet
    workbook.Save(Constants.savePivottablePath + "Template.xlsx");

    //workbook = new Workbook("D:\\mmm.xlsx");//source sheet
    //workbook.Worksheets[0].PivotTables[0].CalculateData();
    //workbook.Save(Constants.savePivottablePath + "m.xlsx");

    //www.aspose.com/community/forums/thread/304764.aspx
    workbook = new Workbook(Constants.openPivottablePath + "Aspose+Attach.XLSM");//source sheet
    workbook.Save(Constants.savePivottablePath + "Aspose+Attach.xlsx");

    //workbook = new Workbook("D:\\e.xlsx");//source sheet
    //Style style = workbook.CreateStyle();
    //style.Rotation = 55;
    //workbook.Worksheets[0].PivotTables[0].Format(8, 6, style);
    //workbook.Save("D:\\tt.xlsx");

    //workbook = new Workbook("D:\\e.xlsx");//source sheet

    //workbook.CalculateFormula();
    //int t = (int)workbook.Worksheets[0].Cells["B16"].Value;

}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


