---
title: "HtmlSaveOptions.CssStyles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta gli stili css aggiuntivi per il formattatore. Funziona solo quando SaveAsSingleFile è True.  CssStylesbody  padding 5px"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Ottiene o imposta gli stili css aggiuntivi per il formattatore. Funziona solo quando [`SaveAsSingleFile`](../saveassinglefile/) è True.  CssStyles=\"body { padding: 5px }\";

```csharp
public string CssStyles { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta stili CSS personalizzati
            saveOptions.CssStyles = @"
                body { 
                    font-family: Arial;
                    background-color: #f0f0f0;
                }
                table {
                    border-collapse: collapse;
                    width: 100%;
                }
                td {
                    border: 1px solid #ddd;
                    padding: 8px;
                }";

            // Salva la cartella di lavoro con stili CSS personalizzati
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


