---
title: "Cell.IsInArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Anger om cellens formel är en matrisformel"
type: docs
url: /sv/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Anger om cellens formel är en matrisformel.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Anmärkningar

OBS: Denna klass är nu föråldrad. Använd istället Cell.IsArrayFormula för att kontrollera om cellens formel är en matrisformel. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata med matrisformler
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Ange en matrisformel med hjälp av rätt API
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // Kontrollera egenskapen IsInArray
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // Visa hur man rensar icke‑matrisceller
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // Spara arbetsboken
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


