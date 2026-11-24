---
title: "HtmlSaveOptions.CssStyles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Ruft die zusätzlichen css-Stile für den Formatter ab oder legt sie fest. Funktioniert nur, wenn SaveAsSingleFile True ist.  CssStylesbody  padding 5px"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Ruft die zusätzlichen css-Stile für den Formatter ab oder legt sie fest. Funktioniert nur, wenn [`SaveAsSingleFile`](../saveassinglefile/) True ist.  CssStyles="body { padding: 5px }";

```csharp
public string CssStyles { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Benutzerdefinierte CSS-Stile festlegen
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

            // Arbeitsmappe mit benutzerdefinierten CSS-Stilen speichern
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


