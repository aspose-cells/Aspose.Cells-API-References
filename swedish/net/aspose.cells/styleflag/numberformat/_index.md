---
title: "StyleFlag.NumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Inställning för talformat kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Inställning för talformat kommer att tillämpas.

```csharp
public bool NumberFormat { get; set; }
```

### Exempel

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
            
            // Ange cellvärde
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Skapa en anpassad talformatstil
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Applicera endast talformat med StyleFlag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Applicera stilen på cellområde (fullständigt kvalificera Range-typ)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Spara och verifiera
            workbook.Save("output_number_format.ods");
            
            // Ladda om för att verifiera
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


