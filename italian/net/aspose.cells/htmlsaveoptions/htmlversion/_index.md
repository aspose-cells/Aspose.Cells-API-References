---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Specifica la versione dello standard HTML da utilizzare durante il salvataggio del formato HTML. Il valore predefinito è HtmlVersion.Default"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

Specifica la versione dello standard HTML da utilizzare quando si salva il formato HTML. Il valore predefinito è HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // Crea un'istanza di HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Visualizza il valore corrente di HtmlVersion
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // Imposta HtmlVersion su HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Salva con la versione HTML5
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // Passa a XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Salva con la versione XHTML
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Ripristina al valore predefinito
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Salva con la versione predefinita
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### Vedi anche

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


