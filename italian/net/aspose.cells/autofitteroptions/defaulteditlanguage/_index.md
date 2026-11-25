---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Ottiene o imposta la lingua di modifica predefinita"
type: docs
url: /it/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Ottiene o imposta la lingua di modifica predefinita.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Osservazioni

Può visualizzare/renderizzare layout diversi per il paragrafo di testo quando è impostata una lingua di modifica diversa. Il valore predefinito è Auto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta testo CJK di esempio in una cella
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Adatta automaticamente la riga con le impostazioni della lingua CJK
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


