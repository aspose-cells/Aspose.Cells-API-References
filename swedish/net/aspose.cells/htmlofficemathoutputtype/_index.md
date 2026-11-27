---
title: "Enum HtmlOfficeMathOutputType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlOfficeMathOutputType-enum. Representerar hur OfficeMath exporteras till HTML"
type: docs
url: /sv/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

Representerar hur man exporterar OfficeMath till HTML.

```csharp
public enum HtmlOfficeMathOutputType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Image | `0` | Konverterar OfficeMath till HTML som bild specificerad av &lt;img&gt;-taggen. |
| MathML | `1` | Konverterar OfficeMath till HTML med hjälp av MathML. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till OfficeMath i cell A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in OfficeMath-utmatningstyp till Bild
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Spara med bildutmatningstyp
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Ändra utmatningstyp till MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // Spara med MathML-utmatningstyp
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


