---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Konstruktor. Erstellt eine Option zum Laden der Datei"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Erstellt eine Option zum Laden der Datei.

```csharp
public HtmlLoadOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen mit dem Konstruktor erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // HTML-Datei mit den Optionen laden
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Daten aus dem geladenen HTML abrufen
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Erstellt eine Option zum Laden der Datei.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | LoadFormat | Das Ladeformat. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // HtmlLoadOptions-Instanz mit dem Konstruktor und dem LoadFormat-Parameter erstellen
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Einige Eigenschaften von HtmlLoadOptions festlegen
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Eine Arbeitsmappe mit den Ladeoptionen erstellen
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];

                // Einige Informationen über das geladene HTML anzeigen
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Speichere die Arbeitsmappe
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


