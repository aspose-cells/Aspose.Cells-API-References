---
title: WorkbookDesigner.ClearDataSource
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. Clears all data sources
type: docs
url: /net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Clears all data sources.

```csharp
public void ClearDataSource()
```

### Examples

```csharp
// Called: myWorkbook.ClearDataSource();
public void WorkbookDesigner_Method_ClearDataSource()
{
    WorkbookDesigner myWorkbook = new WorkbookDesigner();
    //myWorkbook.Open(xlFileName);
    Worksheet curentWorksheet = myWorkbook.Workbook.Worksheets["Sheet1"];

    // Create temporary data
    IList<Person> myList = new List<Person>();
    myList.Add(new Person("X", 26));
    myList.Add(new Person("X", 32));
    myList.Add(new Person("Y", 19));


    // Set the headers and smart markers to the XL file
    curentWorksheet.Cells["A1"].PutValue("Name");
    curentWorksheet.Cells["B1"].PutValue("Age");
    curentWorksheet.Cells["A2"].PutValue("&=Person.Name(group:merge,skip:1)");
    curentWorksheet.Cells["B2"].PutValue("&=Person.Age");

    // Set the data to the XL sheet
    myWorkbook.SetDataSource("Person", myList);

    myWorkbook.Process();
    myWorkbook.ClearDataSource();
    myWorkbook.SetDataSource("Person", myList);
    myWorkbook.Workbook.Save(Constants.destPath + "GroupCustomObjects.xls");
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


