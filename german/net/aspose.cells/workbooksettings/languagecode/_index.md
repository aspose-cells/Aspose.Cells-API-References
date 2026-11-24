---
title: "WorkbookSettings.LanguageCode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt die Benutzeroberflächensprache der Workbook-Version zurück oder legt sie fest, basierend auf dem CountryCode, mit dem die Datei gespeichert wurde."
type: docs
url: /de/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Liest oder setzt die Benutzeroberflächensprache der Workbook-Version basierend auf dem CountryCode, das die Datei gespeichert hat.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Setze den Sprachcode auf Deutsch (Deutschland).
            settings.LanguageCode = CountryCode.Germany;

            // Zeige den aktuellen Sprachcode an.
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Ändere den Sprachcode zu Französisch (Frankreich).
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Speichere die Arbeitsmappe
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


