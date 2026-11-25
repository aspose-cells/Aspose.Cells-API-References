---
title: "Range.ToHtml"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Converte l'intervallo in html"
type: docs
url: /it/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Converti l'intervallo in HTML.

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Opzioni per la conversione dell'intervallo in html. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati nell'intervallo A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Crea un intervallo con il nome di tipo completamente qualificato
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Converti l'intervallo in HTML
            byte[] htmlData = range.ToHtml(options);
            
            // Salva HTML su file
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


