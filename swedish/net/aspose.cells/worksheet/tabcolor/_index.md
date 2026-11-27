---
title: "Worksheet.TabColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar arbetsbladsflikens färg"
type: docs
url: /sv/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Representerar färgen på arbetsbladsfliken.

```csharp
public Color TabColor { get; set; }
```

### Anmärkningar

Denna funktion stöds endast i ExcelXP (Excel2002) och senare versioner. Om du sparar filen som Excel97- eller Excel2000-format kommer den att utelämnas.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in flikfärgen till röd
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Rensa flikfärgen
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Spara den modifierade arbetsboken
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


