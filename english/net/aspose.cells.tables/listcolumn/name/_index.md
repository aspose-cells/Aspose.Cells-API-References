---
title: ListColumn.Name
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the name of the column
type: docs
url: /net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Gets and sets the name of the column.

```csharp
public string Name { get; set; }
```

### Remarks

If sets the name of the column, the according cell' value will be changed too.

### Examples

```csharp
// Called: Assert.AreEqual("40179", worksheet.ListObjects[0].ListColumns[0].Name);
// Excel file opens with warning after using Range.CopyValue for table header
// http://www.aspose.com/community/forums/thread/294623/excel-file-opens-with-warning-after-using-range.copyvalue-for-table-header.aspx
public void ListColumn_Property_Name()
{
    Console.WriteLine("ListColumn_Property_Name()");
    string infn = path + @"example.xlsm";
    string outfn = Constants.destPath + @"example.xlsm";

    Workbook workbook = new Workbook(infn);
    Worksheet worksheet = workbook.Worksheets[0];

    Aspose.Cells.Range rangeSource = worksheet.Cells.CreateRange(0, 0, 1, 3);
    Aspose.Cells.Range rgTeamHeader = worksheet.Cells.CreateRange(2, 0, 1, 3);
    rgTeamHeader.CopyValue(rangeSource);
    Assert.AreEqual("40179", worksheet.ListObjects[0].ListColumns[0].Name);

    workbook.Save(outfn);
}
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


