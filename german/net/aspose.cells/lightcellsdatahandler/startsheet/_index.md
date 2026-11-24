---
title: "LightCellsDataHandler.StartSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataHandler-Methode. Beginnt mit der Verarbeitung eines Arbeitsblatts"
type: docs
url: /de/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

Beginnt mit der Verarbeitung eines Arbeitsblatts.

```csharp
public bool StartSheet(Worksheet sheet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Blatt | Arbeitsblatt | Das Arbeitsblatt, aus dem Zellen­daten gelesen werden. |

### Rückgabewert

Ob die Zellen­daten dieses Arbeitsblatts verarbeitet werden müssen. false, um dieses Arbeitsblatt zu ignorieren.

### Hinweise

Sie wird aufgerufen, bevor die Zellen­daten eines Arbeitsblatts gelesen werden.

### Beispiele

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

### Siehe auch

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


