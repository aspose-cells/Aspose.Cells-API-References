---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om en crosscell-sträng ska visas på samma sätt som i MS Excel när en Excel-fil sparas i html-format. Som standard är värdet Default, så för crosscell-strängar är skillnaden mellan html-filerna som skapas av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora html-filer blir flera gånger snabbare när värdet sätts till Cross jämfört med att sätta det till Default eller Fit2Cell"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Anger om en sträng som sträcker sig över flera celler ska visas på samma sätt som i MS Excel när en Excel-fil sparas i HTML-format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan HTML-filerna som skapas av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora HTML-filer blir flera gånger snabbare om värdet sätts till Cross jämfört med Default eller Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata som demonstrerar beteende över flera strängar
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Hämta och ändra cellstilar
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // Konfigurera HTML‑sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Spara arbetsboken till HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### Se även

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


