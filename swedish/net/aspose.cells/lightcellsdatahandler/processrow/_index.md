---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataHandler-metoden. Påbörjar bearbetning av en rad"
type: docs
url: /sv/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Påbörjar bearbetning av en rad.

```csharp
public bool ProcessRow(Row row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Row | Radobjekt som för närvarande bearbetas. |

### Returvärde

om den här radens celler behöver bearbetas. false för att ignorera alla celler i denna rad.

### Anmärkningar

Den kommer att anropas efter att radens egenskaper såsom höjd, stil, ...etc. har lästs. Dock har cellerna i denna rad ännu inte lästs.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Skapa anpassad hanterare
                var handler = new CustomRowHandler();

                // Bearbeta den första raden
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Demonstrera åtkomst till radens egenskaper
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Ändra radens höjd om den inte är rubrikraden
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Se även

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


