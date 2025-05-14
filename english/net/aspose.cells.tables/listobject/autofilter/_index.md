---
title: ListObject.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets auto filter
type: docs
url: /net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Gets auto filter.

```csharp
public AutoFilter AutoFilter { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(lo.AutoFilter.Range == null, true);//CELLSNET-43054
public void ListObject_Property_AutoFilter()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    Worksheet worksheet = workbook.Worksheets[0];

    ListObject lo = worksheet.ListObjects[0];

    lo.Resize(0, 1, 10, 4, true);
    Assert.AreEqual(worksheet.Cells["D8"].IsFormula, true);//CellsNet43028,43049
    Assert.AreEqual(worksheet.Cells["E8"].GetValidation() != null, true);//43032
    Assert.AreEqual(lo.AutoFilter.Range == null, true);//CELLSNET-43054
    worksheet.Cells["B17"].PutValue("Open the file with xmlspy, check table1.xml,Calculated ColumnFormula should exists.");
    Util.SaveManCheck(workbook, "ExcelUI", "example.xlsx");
           
}
```

### See Also

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


