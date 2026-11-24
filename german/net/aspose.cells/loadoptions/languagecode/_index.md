---
title: "LoadOptions.LanguageCode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem Ländercode zurück oder legt sie fest, unter dem die Datei gespeichert wurde"
type: docs
url: /de/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Liest oder setzt die Benutzeroberflächensprache der Workbook-Version basierend auf dem CountryCode, das die Datei gespeichert hat.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // LanguageCode‑Eigenschaft festlegen
            loadOptions.LanguageCode = CountryCode.USA;

            // Laden Sie eine Arbeitsmappe mit den angegebenen LoadOptions.
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Arbeitsblatt öffnen und Inhalt ändern
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


