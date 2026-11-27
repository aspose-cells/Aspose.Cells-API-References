---
title: "TableStyle.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyle-egenskap. Hämtar namnet på tabellstilen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Hämtar namnet på tabellstil.

```csharp
public string Name { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Få åtkomst till samlingen av tabellstilar
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Hämta den första tabellstilen från samlingen
                TableStyle tableStyle = tableStyles[0];

                // Visa värdet för egenskapen Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Demonstrera åtkomst till den skrivskyddade egenskapen
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Visa att vi kan använda namnet för att referera till stilen
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Spara arbetsboken
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


