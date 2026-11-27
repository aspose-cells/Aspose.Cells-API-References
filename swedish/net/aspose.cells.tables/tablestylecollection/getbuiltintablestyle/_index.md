---
title: "TableStyleCollection.GetBuiltinTableStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleCollection-metod. Hämtar den inbyggda tabellstilen"
type: docs
url: /sv/net/aspose.cells.tables/tablestylecollection/getbuiltintablestyle/
---
## TableStyleCollection.GetBuiltinTableStyle method

Hämtar den inbyggda tabellstilen

```csharp
public TableStyle GetBuiltinTableStyle(TableStyleType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | TableStyleType | Den inbyggda tabellstilstypen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodGetBuiltinTableStyleWithTableStyleTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa en tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Hämta samlingen av tabellstilar
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Anropa GetBuiltinTableStyle med TableStyleType-parameter
                TableStyle builtinStyle = tableStyles.GetBuiltinTableStyle(TableStyleType.TableStyleMedium2);

                // Applicera den inbyggda stilen på vår tabell
                table.TableStyleName = builtinStyle.Name;

                Console.WriteLine($"Applied built-in table style: {builtinStyle.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBuiltinTableStyle method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("TableStyleCollectionMethodGetBuiltinTableStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [TableStyle](../../tablestyle/)
* enum [TableStyleType](../../tablestyletype/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


