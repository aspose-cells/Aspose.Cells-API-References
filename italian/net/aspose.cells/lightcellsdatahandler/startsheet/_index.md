---
title: "LightCellsDataHandler.StartSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataHandler. Inizia a elaborare un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

Inizia a elaborare un foglio di lavoro.

```csharp
public bool StartSheet(Worksheet sheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| foglio | Worksheet | il foglio di lavoro per leggere i dati delle celle. |

### Valore di ritorno

indica se i dati delle celle di questo foglio devono essere elaborati. false per ignorare questo foglio.

### Osservazioni

Verrà chiamato prima di leggere i dati delle celle di un foglio di lavoro.

### Esempi

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

### Vedi anche

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


