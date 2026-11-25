---
title: "Workbook.HasExernalLinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Indica se questo workbook contiene collegamenti esterni ad altre fonti di dati"
type: docs
url: /it/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Indica se questo workbook contiene collegamenti esterni ad altre fonti di dati.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Valore di ritorno

Se questo workbook contiene collegamenti esterni ad altre fonti di dati.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare ExternalLinkCollection.Count per verificare se ci sono collegamenti esterni in questo workbook. Questo metodo sarà rimosso 12 mesi dopo a partire da dicembre 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Crea un workbook con collegamenti esterni
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Aggiungi un collegamento esterno
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Verifica se il workbook ha collegamenti esterni
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


