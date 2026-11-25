---
title: "PaginatedSaveOptions.DefaultEditLanguage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Ottiene o imposta la lingua di modifica predefinita"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

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
    public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi del testo CJK per dimostrare la proprietà DefaultEditLanguage
            worksheet.Cells["A1"].PutValue("日本語のテキスト");
            worksheet.Cells["A2"].PutValue("中文文本");
            worksheet.Cells["A3"].PutValue("한글 텍스트");

            // Crea le opzioni di salvataggio PDF e imposta CJK come lingua di modifica predefinita
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            
            // Salva la cartella di lavoro con le opzioni specificate
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("Workbook saved with CJK as default edit language.");
        }
    }
}
```

### Vedi anche

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


