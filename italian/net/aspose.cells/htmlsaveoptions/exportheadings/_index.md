---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le intestazioni di righe e colonne dei fogli durante il salvataggio in file HTML"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Indica se esportare le intestazioni di righe e colonne del foglio quando si salva in file HTML.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà HtmlSaveOptions.ExportRowColumnHeadings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Crea le opzioni di salvataggio HTML e abilita l'esportazione delle intestazioni
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // Salva come HTML con intestazioni
            workbook.Save("output_with_headings.html", options);
            
            // Salva nuovamente senza intestazioni per confronto
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


