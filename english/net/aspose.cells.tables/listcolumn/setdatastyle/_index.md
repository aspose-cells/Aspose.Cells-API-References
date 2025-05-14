---
title: ListColumn.SetDataStyle
second_title: Aspose.Cells for .NET API Reference
description: ListColumn method. Sets the style of the data in this column of the table
type: docs
url: /net/aspose.cells.tables/listcolumn/setdatastyle/
---
## ListColumn.SetDataStyle method

Sets the style of the data in this column of the table.

```csharp
public void SetDataStyle(Style style)
```

### Examples

```csharp
// Called: table.ListColumns[0].SetDataStyle(style);
public void ListColumn_Method_SetDataStyle()
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


