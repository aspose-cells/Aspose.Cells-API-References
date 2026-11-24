---
title: "PageSetup.PrintErrors"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt den Typ des angezeigten Druckfehlers an."
type: docs
url: /de/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Gibt den Typ des angezeigten Druckfehlers an.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet sheet = workbook.Worksheets[0];
            
            // Stellen Sie Druckfehler so ein, dass sie als leer angezeigt werden.
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Ändern Sie die Druckfehleranzeige zu Strichen.
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


