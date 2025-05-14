---
title: ListColumn.GetDataStyle
second_title: Aspose.Cells for .NET API Reference
description: ListColumn method. Gets the style of the data in this column of the table
type: docs
url: /net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

Gets the style of the data in this column of the table.

```csharp
public Style GetDataStyle()
```

### Examples

```csharp
// Called: Style style = table.ListColumns[0].GetDataStyle();
public void ListColumn_Method_GetDataStyle()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    ListObject table = workbook.Worksheets[0].ListObjects[0];
    Style style = table.ListColumns[0].GetDataStyle();
    style.Pattern = BackgroundType.Solid;
    // style.ForegroundColor = Color.Red;
    style.BackgroundColor = Color.Red;
    table.ListColumns[0].SetDataStyle(style);
    Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].Cells["A3"].GetStyle().ForegroundColor));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


