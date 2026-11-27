---
title: "Class SheetSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.SheetSet-klass. Beskriver en uppsättning blad"
type: docs
url: /sv/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Beskriver en uppsättning blad.

```csharp
public class SheetSet
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Skapar en bladuppsättning baserad på exakta bladindex. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Skapar en bladuppsättning baserad på exakta bladnamn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Hämtar en uppsättning med det aktiva bladet i arbetsboken. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Hämtar en uppsättning med alla blad i arbetsboken i deras ursprungliga ordning. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Hämtar en uppsättning med synliga blad i arbetsboken i deras ursprungliga ordning. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // Skapa ett PdfSaveOptions-objekt
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Ställ in SheetSet-egenskapen så att den endast inkluderar det aktiva bladet
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Spara arbetsboken till en PDF-fil
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Ställ in SheetSet-egenskapen så att den inkluderar alla synliga blad
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Spara arbetsboken till en PDF-fil
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Ställ in SheetSet-egenskapen så att den inkluderar alla blad
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Spara arbetsboken till en PDF-fil
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


