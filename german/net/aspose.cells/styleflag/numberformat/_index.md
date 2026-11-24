---
title: "StyleFlag.NumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung des Zahlenformats wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Die Einstellung für das Zahlenformat wird angewendet.

```csharp
public bool NumberFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Zellwert setzen
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Benutzerdefinierten Zahlenformatstil erstellen
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Nur das Zahlenformat mit StyleFlag anwenden
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Den Stil auf den Zellbereich anwenden (Range-Typ vollständig qualifizieren)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Speichern und überprüfen
            workbook.Save("output_number_format.ods");
            
            // Neu laden, um zu überprüfen
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


