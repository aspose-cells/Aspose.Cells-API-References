---
title: "WorkbookSettings.LanguageCode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro in base a CountryCode con cui è stato salvato il file"
type: docs
url: /it/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Ottiene o imposta la lingua dell'interfaccia utente della versione del Workbook basata sul CountryCode che ha salvato il file.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta il codice lingua su Tedesco (Germania)
            settings.LanguageCode = CountryCode.Germany;

            // Visualizza il codice lingua corrente
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Cambia il codice lingua in Francese (Francia)
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Salva la cartella di lavoro
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


