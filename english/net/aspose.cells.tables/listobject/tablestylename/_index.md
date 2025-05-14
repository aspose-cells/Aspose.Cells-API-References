---
title: ListObject.TableStyleName
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the table style name
type: docs
url: /net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

Gets and sets the table style name.

```csharp
public string TableStyleName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("TableStyleLight15", table.TableStyleName);
public void ListObject_Property_TableStyleName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    ListObject table = workbook.Worksheets[0].ListObjects[0];
    Assert.AreEqual("TableStyleLight15", table.TableStyleName);
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


