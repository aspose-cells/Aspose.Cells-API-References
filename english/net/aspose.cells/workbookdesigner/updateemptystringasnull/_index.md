---
title: WorkbookDesigner.UpdateEmptyStringAsNull
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. If TRUE Null will be inserted if the value is 
type: docs
url: /net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

If TRUE, Null will be inserted if the value is "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Examples

```csharp
// Called: designer.UpdateEmptyStringAsNull = true;
public void WorkbookDesigner_Property_UpdateEmptyStringAsNull()
{
    DataSet ds1 = new DataSet();
    ds1.ReadXml(Constants.sourcePath + "example.xml");

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    // Instantiate a new WorkbookDesigner 
    WorkbookDesigner designer = new WorkbookDesigner();
    designer.UpdateReference = true;
    designer.UpdateEmptyStringAsNull = true;

    // Specify the Workbook 
    designer.Workbook = workbook;

    designer.SetDataSource(ds1.Tables["underliers"]);
    designer.Process();

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


