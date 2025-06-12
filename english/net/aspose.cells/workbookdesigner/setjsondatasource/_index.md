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
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample marker in cell A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Create workbook designer
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Sample JSON data
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // Set JSON data source
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Process the markers
            designer.Process();
            
            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


