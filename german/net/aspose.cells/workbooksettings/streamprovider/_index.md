---
title: "WorkbookSettings.StreamProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings‑Eigenschaft. Gibt den Stream‑Provider für externe Ressourcen zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

Gibt den Stream‑Provider für externe Ressourcen zurück und legt ihn fest.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die ResourceProvider‑Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juni 2022 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Zeige den aktuellen StreamProvider‑Wert an
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // Setze einen benutzerdefinierten Stream‑Provider
            settings.StreamProvider = new CustomStreamProvider1();

            // Füge einige Daten hinzu, um die Verwendung von Stream zu demonstrieren
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // Speichere die Arbeitsmappe – dies löst den Stream‑Provider aus
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // Setze den Stream‑Provider zurück
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### Siehe auch

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


