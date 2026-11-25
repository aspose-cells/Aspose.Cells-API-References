---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // Configura le opzioni di salvataggio HTML con IsJsBrowserCompatible impostato su true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // Salva la cartella di lavoro con compatibilità JavaScript
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


