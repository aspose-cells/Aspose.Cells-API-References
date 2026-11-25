---
title: "HtmlSaveOptions.LinkTargetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica il tipo di attributo target in un collegamento. Il valore predefinito è HtmlLinkTargetType.Parent."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

Indica il tipo di attributo target nel link `<a>`. Il valore predefinito è HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Link to Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");

            // Imposta le opzioni di salvataggio HTML con LinkTargetType.
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            // Salva la cartella di lavoro come HTML
            workbook.Save("output.html", saveOptions);
        }
    }
}
```

### Vedi anche

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


