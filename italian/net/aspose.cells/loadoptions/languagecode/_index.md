---
title: "LoadOptions.LanguageCode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta la lingua dell'interfaccia utente della versione del Workbook basata sul CountryCode che ha salvato il file"
type: docs
url: /it/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Ottiene o imposta la lingua dell'interfaccia utente della versione del Workbook basata sul CountryCode che ha salvato il file.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Esempi

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
            // Crea un'istanza di LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Imposta la proprietà LanguageCode
            loadOptions.LanguageCode = CountryCode.USA;

            // Carica una cartella di lavoro con le LoadOptions specificate
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Accedi al foglio di lavoro e modifica il contenuto
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Salva la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


