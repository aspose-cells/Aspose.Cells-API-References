---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DifLoadOptions‑Konstruktor. Die Optionen"
type: docs
url: /de/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Die Optionen.

```csharp
public DifLoadOptions()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine neue Instanz von DifLoadOptions mit dem parameterlosen Konstruktor
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Erstelle ein neues Arbeitsbuch mit Standardoptionen
                Workbook workbook = new Workbook();

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];

                // Füge Beispieldaten hinzu, um zu demonstrieren, dass das Arbeitsbuch funktionsfähig ist
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Arbeitsmappe im DIF-Format speichern
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Lade nun die gespeicherte DIF‑Datei mit DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Die geladenen Daten zur Überprüfung als XLSX speichern
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


