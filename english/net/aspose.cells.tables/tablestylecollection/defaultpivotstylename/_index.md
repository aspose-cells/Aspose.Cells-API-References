---
title: TableStyleCollection.DefaultPivotStyleName
second_title: Aspose.Cells for .NET API Reference
description: TableStyleCollection property. Gets and sets the default style name of pivot table 
type: docs
url: /net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Gets and sets the default style name of pivot table .

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("PivotStyleLight16", tableStyles.DefaultPivotStyleName);
public void TableStyleCollection_Property_DefaultPivotStyleName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
    Assert.AreEqual("TableStyleDark3", tableStyles.DefaultTableStyleName);
    Assert.AreEqual("PivotStyleLight16", tableStyles.DefaultPivotStyleName);

    tableStyles.DefaultTableStyleName = "TableStyleMedium9";
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    tableStyles = workbook.Worksheets.TableStyles;
    Assert.AreEqual("TableStyleMedium9", tableStyles.DefaultTableStyleName);
}
```

### See Also

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


