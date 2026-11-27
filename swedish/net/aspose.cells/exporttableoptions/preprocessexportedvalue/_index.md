---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions metod. Förbehandla värdet på den aktuella cellen som ska exporteras"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Förprocessa värdet i den aktuella cellen som ska exporteras.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellRow | Int32 | radindex för den aktuella cellen |
| cellColumn | Int32 | kolumnindex för cellen |
| värde | CellValue | värde och typ för den aktuella cellen |

### Returvärde

Om den aktuella cellen har ersatts med en annan typ och/eller värde.

### Anmärkningar

Rad- och kolumnindex är cellens absoluta index i kalkylbladet, inte index i den exporterade tabellen. Användaren kan kontrollera värdet på den aktuella cellen i den överskrivna implementeringen av denna metod; om den aktuella cellen behöver ersättas med en annan typ och värde, bör implementeringen här sätta den förväntade typen och värdet på CellValue‑objektet och returnera true. Som standard gör denna metod ingenting och returnerar false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Skapa en instans av ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Skapa ett CellValue‑objekt för demonstration
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // Anropa PreprocessExportedValue med specifika parametrar (rad 0, kolumn 0, CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Visa resultatet av metodanropet
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // Modifiera cellen med det bearbetade värdet om det behövs
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Spara arbetsboken
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


