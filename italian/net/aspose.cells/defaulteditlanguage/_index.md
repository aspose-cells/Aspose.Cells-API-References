---
title: "Enum DefaultEditLanguage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.DefaultEditLanguage. Rappresenta la lingua di modifica predefinita"
type: docs
url: /it/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Rappresenta la lingua di modifica predefinita.

```csharp
public enum DefaultEditLanguage
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Auto | `0` | Rappresenta il rilevamento automatico della lingua di modifica in base al testo stesso. |
| English | `1` | Rappresenta la lingua inglese. |
| CJK | `2` | Rappresenta le lingue cinese, giapponese e coreana. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea AutoFitterOptions e imposta DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Applica l'adattamento automatico delle righe con le opzioni specificate
            worksheet.AutoFitRows(autoFitterOptions);

            // Salva la cartella di lavoro
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Stampa su console il DefaultEditLanguage impostato
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


