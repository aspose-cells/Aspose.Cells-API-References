---
title: Worksheet.Name
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets the name of the worksheet
type: docs
url: /net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Gets or sets the name of the worksheet.

```csharp
public string Name { get; set; }
```

### Remarks

The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### Examples

```csharp
// Called: sheetDest.Name = "sheetDest";
[Test, Ignore("Not ready to test this yet")]
        public void Property_Name()
        {
            caseName = "testRangeCopyStyle_Chart";
            Workbook workbook = new Workbook(Constants.sourcePath + "Copy//testChart_003.xls");
            Worksheet sheetSrc = workbook.Worksheets["Chart"];
            Cells cellsSrc = sheetSrc.Cells;
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(0, 0, 26, 11);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(0, 0, 26, 11);
            rangeDest.CopyStyle(rangeSrc);

            checkRangeCopyStyle_Chart(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xls");            
            workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xls");
            checkRangeCopyStyle_Chart(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xlsx");
            workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xlsx");
            checkRangeCopyStyle_Chart(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xml");
            checkRangeCopyStyle_Chart(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xls");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


