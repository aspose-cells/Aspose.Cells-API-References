---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner‑Methode. Gibt eine Sammlung von Smart‑Markern in einer Tabellenkalkulation zurück"
type: docs
url: /de/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Gibt eine Sammlung von Smart‑Markern in einer Tabellenkalkulation zurück.

```csharp
public string[] GetSmartMarkers()
```

### Rückgabewert

Eine Sammlung von Smart‑Markern

### Hinweise

Ein String‑Array wird bei jedem Aufruf erstellt. Das Array wird sortiert und duplizierte Werte werden entfernt.

### Beispiele

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Beispielvorlagendatei im Speicher
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Fügen Sie Smart‑Marker zur Vorlage hinzu
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Speichern Sie die Vorlage in einen Memory‑Stream
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // Initialisieren Sie WorkbookDesigner mit der Vorlage
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Abrufen und Anzeigen von Smart‑Markern
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Datenquelle vorbereiten
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Setze Datenquelle und verarbeite
            designer.SetDataSource(data);
            designer.Process();
            
            // Ergebnis speichern
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


