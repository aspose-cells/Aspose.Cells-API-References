---
title: "HtmlSaveOptions.LinkTargetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt den Typ des target-Attributs in einem Link an. Der Standardwert ist HtmlLinkTargetType.Parent."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

Gibt den Typ des target‑Attributs in einem `<a>`‑Link an. Der Standardwert ist HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Link to Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");

            // HTML-Speicheroptionen mit LinkTargetType festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            // Speichere die Arbeitsmappe als HTML
            workbook.Save("output.html", saveOptions);
        }
    }
}
```

### Siehe auch

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


