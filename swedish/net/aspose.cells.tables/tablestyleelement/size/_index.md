---
title: "TableStyleElement.Size"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleElement-egenskap. Antal rader eller kolumner i ett enda band av ränder. Gäller endast när typ är firstRowStripe secondRowStripe firstColumnStripe eller secondColumnStripe"
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Antal rader eller kolumner i ett enda band av ränder. Gäller endast när typen är firstRowStripe, secondRowStripe, firstColumnStripe eller secondColumnStripe.

```csharp
public int Size { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Skapa en tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Skapa en tabellstil med arbetsbokens stilssamling
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Lägg till randelement för att demonstrera Size-egenskapen
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Åtkomst till randelementen
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Visa aktuella Size-värden
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Ändra randstorlekarna
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Visa ändrade värden
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Spara arbetsboken för att se effekterna
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


