---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-metod. Ange json-strängvärde som datakälla för smarta markörer"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

Ange JSON‑strängvärde som datakälla för smart markers.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på tabellen. Om värdet av JSON representerar ett objekt kan det vara null. |
| json | String | Värdet av Json-strängen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett exempelmarkör i cell A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Skapa arbetsboksdesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Exempel på JSON‑data
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // Ange JSON-datakälla
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Bearbeta markörerna
            designer.Process();
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


