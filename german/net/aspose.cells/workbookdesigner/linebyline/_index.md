---
title: "WorkbookDesigner.LineByLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Eigenschaft. Gibt an, ob der Smart Marker zeilenweise verarbeitet wird"
type: docs
url: /de/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Gibt an, ob der Smart Marker zeilenweise verarbeitet wird.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Hinweise

Der Standardwert ist true. Wenn False, muss die Vorlagendatei einen Bereich enthalten, der "_CellsSmartMarkers" genannt wird.

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Bereich‑Smart‑Marker. Diese Eigenschaft wird 12 Monate später, seit Juli 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Beispielarbeitsmappe mit Smart‑Markern
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Richten Sie Smart‑Marker im Arbeitsblatt ein
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Erstelle Beispieldaten
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // Verarbeiten Sie mit LineByLine auf false gesetzt
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Ergebnis speichern
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Einfache Datenklasse zur Demonstration
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


