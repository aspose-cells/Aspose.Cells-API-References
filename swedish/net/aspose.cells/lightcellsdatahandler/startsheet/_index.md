---
title: "LightCellsDataHandler.StartSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataHandler-metoden. Påbörjar bearbetning av ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

Påbörjar bearbetning av ett kalkylblad.

```csharp
public bool StartSheet(Worksheet sheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blad | Arbetsblad | kalkylbladet för att läsa celldata. |

### Returvärde

om detta bladets celldata behöver bearbetas. false för att ignorera detta blad.

### Anmärkningar

Den kommer att anropas innan celldata läses för ett kalkylblad.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartSheetWithWorksheetDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                CustomLightCellsDataHandler handler = new CustomLightCellsDataHandler();
                bool result = handler.StartSheet(worksheet);

                Console.WriteLine($"StartSheet method returned: {result}");
                Console.WriteLine($"Worksheet name after StartSheet: {worksheet.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }

            workbook.Save("LightCellsDataHandlerStartSheetDemo.xlsx");
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            sheet.Name = "ModifiedByStartSheet";
            return true;
        }

        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


