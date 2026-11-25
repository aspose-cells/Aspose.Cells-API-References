---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false

```csharp
public bool IsIECompatible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta la proprietà IsIECompatible
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // Salva la cartella di lavoro con le opzioni HTML
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


