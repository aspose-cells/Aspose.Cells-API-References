---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLayoutOptions-Eigenschaft. Gibt an, ob der Titel ignoriert wird, wenn das Objekt eine Eigenschaft eines anderen Objekts ist"
type: docs
url: /de/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Gibt an, ob der Titel ignoriert wird, wenn das Objekt eine Eigenschaft eines anderen Objekts ist.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
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

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispiel-JSON-Daten mit Objekttiteln
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // JsonLayoutOptions erstellen
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Aktuellen IgnoreObjectTitle-Wert anzeigen
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Auf Ignorieren von Objekttiteln setzen
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // JSON mit IgnoreObjectTitle = true importieren
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Speichern mit ignorierten Titeln
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Setze das Arbeitsblatt zurück
            worksheet.Cells.Clear();

            // Einstellen, Objekt‑Titel einzuschließen
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // JSON importieren mit IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Speichern mit eingeschlossenen Titeln
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### Siehe auch

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


