---
title: "PageSetup.Order"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Reihenfolge an, die Microsoft Excel beim Nummerieren von Seiten verwendet, wenn ein großes Arbeitsblatt gedruckt wird."
type: docs
url: /de/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Stellt die Reihenfolge dar, die Microsoft Excel beim Nummerieren von Seiten verwendet, wenn ein großes Arbeitsblatt gedruckt wird.

```csharp
public PrintOrderType Order { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Setzen Sie die Druckreihenfolge auf DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Speichern Sie die Arbeitsmappe in verschiedenen Formaten
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Ändern Sie die Druckreihenfolge zu OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Speichern Sie erneut mit verschiedenen Formaten
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Siehe auch

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


