---
title: "LightCellsDataHandler.StartRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataHandler‑metod. Förbereder att bearbeta en rad"
type: docs
url: /sv/net/aspose.cells/lightcellsdatahandler/startrow/
---
## LightCellsDataHandler.StartRow method

Förbereder bearbetning av en rad.

```csharp
public bool StartRow(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | index för nästa rad som ska bearbetas |

### Returvärde

om den här raden (egenskaper eller celldata) behöver bearbetas. false för att ignorera denna rad och dess celler och kontrollera nästa rad.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartRowWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                using (Workbook workbook = new Workbook())
                {
                    Worksheet sheet = workbook.Worksheets[0];
                    for (int i = 0; i < 5; i++)
                    {
                        sheet.Cells[i, 0].Value = $"Row {i + 1}";
                    }
                    workbook.Save("input.xlsx");
                }

                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
                
                using (Workbook workbook = new Workbook("input.xlsx", loadOptions))
                {
                    workbook.Save("output.xlsx");
                }

                Console.WriteLine("Method executed successfully. Rows with even indices processed.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartRow(int rowIndex)
            {
                return rowIndex % 2 == 0;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool ProcessRow(Row row) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Se även

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


