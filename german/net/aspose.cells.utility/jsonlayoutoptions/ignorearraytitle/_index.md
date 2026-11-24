---
title: "JsonLayoutOptions.IgnoreArrayTitle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLayoutOptions-Eigenschaft. Gibt an, ob der Titel ignoriert wird, wenn das Array eine Eigenschaft des Objekts ist"
type: docs
url: /de/net/aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/
---
## JsonLayoutOptions.IgnoreArrayTitle property

Gibt an, ob der Titel ignoriert wird, wenn das Array eine Eigenschaft des Objekts ist.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreArrayTitle { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die JsonLayoutOptions.IgnoreTitle-Eigenschaft. Diese Eigenschaft wird 6 Monate nach Februar 2023 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreArrayTitleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispiel-JSON-Daten mit Array-Titeln
            string json = @"{
                ""Employees"": [
                    { ""Name"": ""John"", ""Age"": 30 },
                    { ""Name"": ""Jane"", ""Age"": 25 }
                ]
            }";

            // JsonLayoutOptions erstellen
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Aktuellen IgnoreArrayTitle-Wert anzeigen
            Console.WriteLine("Current IgnoreArrayTitle value: " + options.IgnoreArrayTitle);

            // Erster Import mit IgnoreArrayTitle = false (Standardwert)
            options.IgnoreArrayTitle = false;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=false. Check cell A1 for 'Employees' title.");

            // Arbeitsblatt für zweiten Import leeren
            worksheet.Cells.Clear();

            // Zweiter Import mit IgnoreArrayTitle = true
            options.IgnoreArrayTitle = true;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=true. Check cell A1 for direct array values.");

            // Speichere die Arbeitsmappe
            workbook.Save("JsonLayoutOptionsIgnoreArrayTitleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


