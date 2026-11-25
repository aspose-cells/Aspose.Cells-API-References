---
title: "Enum MarkdownTableHeaderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Markdown.MarkdownTableHeaderType. Rappresenta il tipo di intestazione della tabella nel file markdown"
type: docs
url: /it/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Rappresenta il tipo di intestazione della tabella nel file markdown.

```csharp
public enum MarkdownTableHeaderType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| FirstRow | `0` | Prima riga come intestazione della tabella. |
| ColumnHeader | `1` | Nome colonna (come A,B,C...) come intestazione della tabella. |
| Empty | `2` | Una riga di intestazione vuota. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Imposta le opzioni di salvataggio Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Salva come file Markdown
            workbook.Save("output.md", saveOptions);
            
            // Verifica l'output
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


