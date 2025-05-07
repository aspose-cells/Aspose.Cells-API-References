---
title: PivotField.IsAscendSort
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is autosorted ascending
type: docs
url: /net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Indicates whether the specified PivotTable field is autosorted ascending.

```csharp
public bool IsAscendSort { get; set; }
```

### Examples

```csharp
// Called: pTable.RowFields[2].IsAscendSort = false;
[Test]
        public void Property_IsAscendSort()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46387_";

            Workbook wb = new Workbook(filePath + @"UnsortedSamleData1.xlsb");
            Worksheet ws = wb.Worksheets[1];
            var pTable = ws.PivotTables[0];
            //pTable.RefreshData();
            //Sort column LTM Jan-17 by Account Description row 
            pTable.RowFields[2].IsAutoSort = true;
            pTable.RowFields[2].IsAscendSort = false;
            pTable.RowFields[2].AutoSortField = 43;


            pTable.DataFields["LTM Jan-17"].IsAscendSort = false;
            pTable.DataFields["LTM Jan-17"].IsAutoSort = true;

            pTable.RefreshDataOnOpeningFile = true;
            pTable.CalculateData();

            string savePath = CreateFolder(filePath);
            wb.Save(savePath + @"out.Xlsb", SaveFormat.Xlsb);
            wb.Save(savePath + @"out.Xlsx", SaveFormat.Xlsx);

            wb = new Workbook(savePath + "out.Xlsb");
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].RowFields[2].IsAscendSort, false);
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].RowFields[2].AutoSortField, 43);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


