---
title: "HtmlLoadOptions.ProgId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt die Programm-ID beim Erstellen der Datei zurück. Nur für MHT-Dateien"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Liest die Programm‑ID, mit der die Datei erstellt wurde. Nur für MHT‑Dateien.

```csharp
public string ProgId { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen im MHTML-Format erstellen
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // ProgId-Eigenschaft abrufen
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Eine weitere Instanz erstellen und deren ProgId abrufen
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


