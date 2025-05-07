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
// Called: lobj.AutoFilter.AddFilter(0, "1"); //Check the value 2
[Test]
        public void Property_AutoFilter()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet40743.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            ListObject lobj = worksheet.ListObjects[0];
            //Add filter in first column
            lobj.AutoFilter.AddFilter(0, "1"); //Check the value 2
            lobj.AutoFilter.AddFilter(0, "2"); //Check the value 2
            lobj.AutoFilter.Refresh();
            //workbook.Save(Constants.destPath + "CellsNet40743.xls");
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);// new Workbook(Constants.destPath + "CellsNet40743.xls");
            worksheet = workbook.Worksheets[0];
            lobj = worksheet.ListObjects[0];
            // Assert.AreEqual(lobj.AutoFilter.FilterColumns[0].FilterType, FilterType.MultipleFilters);
            Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + "CellsNet40743.xlsx");
        }
```

### See Also

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


