---
title: "StyleFlag.FontUnderline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Inställning för teckensnitt understrykning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

Inställning för understrykning i teckensnittet kommer att tillämpas.

```csharp
public bool FontUnderline { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Skapa ett stilobjekt och ange teckensnitt understrykning
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Skapa en stilflagga och aktivera teckensnitt understrykning-flagga
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Applicera stilen på cellen med stilflaggan
            cell.SetStyle(style, styleFlag);

            // Visa aktuell understrykningsstatus
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Ändra understrykningstypen till dubbel
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Spara arbetsboken
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


