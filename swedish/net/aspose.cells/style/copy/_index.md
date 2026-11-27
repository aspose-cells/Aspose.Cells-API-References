---
title: "Style.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Kopierar data från ett annat stilobjekt"
type: docs
url: /sv/net/aspose.cells/style/copy/
---
## Style.Copy method

Kopierar data från ett annat stilobjekt

```csharp
public void Copy(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Käll-Style-objekt |

### Anmärkningar

Den här metoden kopierar inte stilens namn. Om du vill kopiera namnet, anropa följande kod efter att ha kopierat stilen: destStyle.Name = style.Name.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Skapa källarbetsbok med exempeldata
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kopiera stilen från källan till destinationen
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Applicera den kopierade stilen
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Spara resultatet
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


