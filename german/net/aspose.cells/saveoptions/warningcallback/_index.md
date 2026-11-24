---
title: "SaveOptions.WarningCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt den Warnungs-Callback zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

Liest oder setzt den Warnungs-Callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Erstelle Speicheroptionen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Benutzerdefinierten Warnungs-Callback festlegen
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Dies erzeugt eine Warnung über ein nicht unterstütztes Feature im HTML-Format
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Speichern mit Optionen, die Warnungen auslösen könnten
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Warnung behandeln – in diesem Fall einfach anzeigen
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### Siehe auch

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


