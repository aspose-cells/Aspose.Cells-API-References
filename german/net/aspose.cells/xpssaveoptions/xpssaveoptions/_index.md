---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XpsSaveOptions-Konstruktor. Erstellt Optionen zum Speichern einer XPS-Datei"
type: docs
url: /de/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Erstellt Optionen zum Speichern von Xps-Dateien.

```csharp
public XpsSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Initialisieren von XpsSaveOptions mit dem Konstruktor
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Speicheroptionen konfigurieren
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Arbeitsmappe mit Optionen speichern
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### Siehe auch

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Erstellt Optionen zum Speichern von Xps-Dateien.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Speicherformat, es muss das XPS-Format sein. |

### Hinweise

HINWEIS: Dieser Konstruktor ist jetzt veraltet. Verwenden Sie stattdessen den XpsSaveOptions()-Konstruktor. Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // Erstellen Sie XpsSaveOptions mit dem Konstruktor und dem SaveFormat-Parameter
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // Speichere die Arbeitsmappe mit den angegebenen Optionen
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


