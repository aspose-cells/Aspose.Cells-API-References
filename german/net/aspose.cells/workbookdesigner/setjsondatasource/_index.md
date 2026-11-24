---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Methode. Setzen Sie den json-Zeichenfolgenwert als Datenquelle für Smart-Marker"
type: docs
url: /de/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

Setzt den JSON‑Stringwert als Datenquelle für Smart‑Marker.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Tabelle. Wenn der Wert von JSON ein Objekt darstellt, kann er null sein. |
| json | String | Der Wert der Json-Zeichenfolge. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einen Beispielmarker in Zelle A1 hinzu
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // WorkbookDesigner erstellen
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Beispieldaten für JSON
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // JSON-Datenquelle festlegen
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Verarbeiten Sie die Marker
            designer.Process();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


