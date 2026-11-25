---
title: "Enum HtmlVersion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.HtmlVersion. Indica la versione di HTML utilizzata durante il salvataggio nei formati Html."
type: docs
url: /it/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

Indica la versione di HTML utilizzata quando si salva nei formati HTML.

```csharp
public enum HtmlVersion
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Salva il documento in conformità con l'esportazione HTML di MS Excel. |
| XHtml | `1` | Salva il documento in conformità con lo standard XHTML 1.0 Transitional. |
| Html5 | `2` | Salva il documento in conformità con lo standard HTML 5. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Imposta la versione HTML su HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Salva la cartella di lavoro con la versione HTML5
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // Cambia la versione HTML in XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Salva la cartella di lavoro con la versione XHTML
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // Imposta la versione HTML su Predefinita (compatibile con MS Excel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Salva la cartella di lavoro con la versione Predefinita
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


