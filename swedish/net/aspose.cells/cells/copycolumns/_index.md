---
title: "Cells.CopyColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Kopierar data och format för en hel kolumn"
type: docs
url: /sv/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Kopierar data och format för en hel kolumn.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceColumnIndex | Int32 | Källkolumnindex. |
| destinationColumnIndex | Int32 | Destinationskolumnindex. |
| columnNumber | Int32 | Numret på den kopierade kolumnen. |
| pasteOptions | PasteOptions | alternativen för inklistring. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Skapa en annan arbetsbok som destination
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Kopiera kolumner med enbart formatering
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Spara arbetsboken
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Kopierar data och format för hela kolumner.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceColumnIndex | Int32 | Källkolumnindex. |
| destinationColumnIndex | Int32 | Destinationskolumnindex. |
| columnNumber | Int32 | Numret på den kopierade kolumnen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata i kolumner
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Kopiera kolumner från kolumnindex 1 (B) till kolumnindex 3 (D), kopiera 1 kolumn
            cells.CopyColumns(cells, 1, 3, 1);

            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Kopierar data och format för de hela kolumnerna.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceColumnIndex | Int32 | Källkolumnindex. |
| sourceTotalColumns | Int32 | Antalet källkolumner. |
| destinationColumnIndex | Int32 | Destinationskolumnindex. |
| destinationTotalColumns | Int32 | Antalet destinationskolumner. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i källkolumner (kolumner 0 och 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // Kopiera 2 kolumner från index 0 till destinationsindex 3, infoga 2 kolumner
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Verifiera kopieringen genom att kontrollera destinationskolumner (3 och 4)
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


