---
title: Range.Name
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets or sets the name of the range
type: docs
url: /net/aspose.cells/range/name/
---
## Range.Name property

Gets or sets the name of the range.

```csharp
public string Name { get; set; }
```

### Remarks

Named range is supported. For example,

range.Name = "Sheet1!MyRange";

### Examples

```csharp
// Called: range.Name = "testRange";
public void Range_Property_Name()
{
    caseName = "testCreateRange_001";
    Workbook workbook = new Workbook(FileFormatType.Excel97To2003);
    Cells cells = workbook.Worksheets[0].Cells;
    Aspose.Cells.Range range = cells.CreateRange(0, 2, true); //=Sheet1!$A:$B
    range.Name = "testRange";

    checkCreateRange_001(workbook, 65536);
    workbook.Save(Constants.destPath + "testCreateRange.xls");
    workbook = new Workbook(Constants.destPath + "testCreateRange.xls");
    checkCreateRange_001(workbook, 65536);
    workbook.Save(Constants.destPath + "testCreateRange.xlsx");
    workbook = new Workbook(Constants.destPath + "testCreateRange.xlsx");
    checkCreateRange_001(workbook, 1048576);
//    SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
//    {
//        LimitAsXls = true
//};
//    workbook.Save(Constants.destPath + "testCreateRange.xml", saveOptions);            
//    workbook = new Workbook(Constants.destPath + "testCreateRange.xml");
//    checkCreateRange_001(workbook,65536);
    workbook.Save(Constants.destPath + "testCreateRange.xls");           
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


