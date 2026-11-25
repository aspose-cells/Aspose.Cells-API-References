---
title: "LightCellsDataHandler.StartRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataHandler. Prepara l'elaborazione di una riga"
type: docs
url: /it/net/aspose.cells/lightcellsdatahandler/startrow/
---
## LightCellsDataHandler.StartRow method

Prepara l'elaborazione di una riga.

```csharp
public bool StartRow(int rowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | l'indice della prossima riga da elaborare |

### Valore di ritorno

se questa riga (proprietà o dati delle celle) deve essere elaborata. false per ignorare questa riga e le sue celle e controllare la riga successiva.

### Esempi

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

### Vedi anche

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


