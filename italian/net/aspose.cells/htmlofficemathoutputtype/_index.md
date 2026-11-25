---
title: "Enum HtmlOfficeMathOutputType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.HtmlOfficeMathOutputType. Rappresenta come esportare OfficeMath in HTML"
type: docs
url: /it/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

Rappresenta come esportare OfficeMath in HTML.

```csharp
public enum HtmlOfficeMathOutputType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Image | `0` | Converte OfficeMath in HTML come immagine specificata dal tag &lt;img&gt;. |
| MathML | `1` | Converte OfficeMath in HTML usando MathML. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi OfficeMath alla cella A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta il tipo di output di OfficeMath su Immagine
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Salva con tipo di output Immagine
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Cambia il tipo di output in MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // Salva con tipo di output MathML
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


