---
title: PivotField.AutoSortField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the index of field which is auto sorted. 1 means PivotField itselfothers means the position of the data fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

```csharp
public int AutoSortField { get; set; }
```

### Examples

```csharp
// Called: pTable.RowFields[2].AutoSortField = 43;
[Test]
        public void Property_AutoSortField()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46387_&quot;;

            Workbook wb = new Workbook(filePath + @&quot;UnsortedSamleData1.xlsb&quot;);
            Worksheet ws = wb.Worksheets[1];
            var pTable = ws.PivotTables[0];
            //pTable.RefreshData();
            //Sort column LTM Jan-17 by Account Description row 
            pTable.RowFields[2].IsAutoSort = true;
            pTable.RowFields[2].IsAscendSort = false;
            pTable.RowFields[2].AutoSortField = 43;


            pTable.DataFields[&quot;LTM Jan-17&quot;].IsAscendSort = false;
            pTable.DataFields[&quot;LTM Jan-17&quot;].IsAutoSort = true;

            pTable.RefreshDataOnOpeningFile = true;
            pTable.CalculateData();

            string savePath = CreateFolder(filePath);
            wb.Save(savePath + @&quot;out.Xlsb&quot;, SaveFormat.Xlsb);
            wb.Save(savePath + @&quot;out.Xlsx&quot;, SaveFormat.Xlsx);

            wb = new Workbook(savePath + &quot;out.Xlsb&quot;);
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].RowFields[2].IsAscendSort, false);
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].RowFields[2].AutoSortField, 43);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


