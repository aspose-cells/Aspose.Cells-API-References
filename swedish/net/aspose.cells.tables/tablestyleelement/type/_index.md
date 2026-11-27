---
title: "TableStyleElement.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleElement-egenskap. Hämtar elementtypen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Hämtar elementtypen.

```csharp
public TableStyleElementType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa en tabell
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Hämta tabellstilen (använd stilnamnet istället för att skapa en ny)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Åtkomst till tabellstilelement
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Visa elementets aktuella typ
            Console.WriteLine("Current Type value: " + element.Type);

            // Obs: Type-egenskapen är skrivskyddad, så vi kan inte sätta den
            // element.Type = TableStyleElementType.TotalRow; // Detta skulle orsaka kompileringsfel

            // Demonstrera hur olika elementtyper påverkar tabellen
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Spara arbetsboken
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


