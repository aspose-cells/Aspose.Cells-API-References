---
title: WorkbookDesigner.Workbook
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Gets and sets the Workbook object
type: docs
url: /net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Gets and sets the `Workbook` object.

```csharp
public Workbook Workbook { get; set; }
```

### Examples

```csharp
// Called: designer.Workbook = new Workbook(Constants.sourcePath + "example.xls");
public void WorkbookDesigner_Property_Workbook()
{
    WorkbookDesigner designer = new WorkbookDesigner();
    //designer.Open(Constants.sourcePath + "example.xls");
    designer.Workbook = new Workbook(Constants.sourcePath + "example.xls");
    System.Collections.Generic.ICollection<Person> list = new System.Collections.Generic.List<Person>();
    list.Add(new Person("simon", 30));
    list.Add(new Person("Johnson", 33));
    designer.SetDataSource("Person", list);
    designer.Process(false);
    Cells cells = designer.Workbook.Worksheets["CustomObjects"].Cells;
    Assert.AreEqual(cells["A2"].StringValue, "simon");
    Assert.AreEqual(cells["A3"].StringValue, "Johnson");
    designer.Workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


