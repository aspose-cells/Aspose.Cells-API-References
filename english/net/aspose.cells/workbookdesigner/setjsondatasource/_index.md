---
title: WorkbookDesigner.SetJsonDataSource
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. 
type: docs
url: /net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

```csharp
public void SetJsonDataSource(string variable, string data)
```

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String |  |
| data | String |  |

### Examples

```csharp
// Called: designer.SetJsonDataSource("c8", jsonData);
public void WorkbookDesigner_Method_SetJsonDataSource()
{
    Workbook wb = new Workbook(Constants.sourcePath + @"example.xlsx");
    WorkbookDesigner designer = new WorkbookDesigner();
    designer.Workbook = wb;
    String jsonData = File.ReadAllText(Constants.sourcePath + @"example.json");
    designer.SetJsonDataSource("c8", jsonData);
    designer.Process();
    wb.Save(Constants.destPath + @"example.xlsx");

}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


