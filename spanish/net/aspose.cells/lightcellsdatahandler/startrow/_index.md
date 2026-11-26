---
title: "LightCellsDataHandler.StartRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataHandler. Prepara el procesamiento de una fila"
type: docs
url: /es/net/aspose.cells/lightcellsdatahandler/startrow/
---
## LightCellsDataHandler.StartRow method

Prepara procesar una fila.

```csharp
public bool StartRow(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | el índice de la siguiente fila a procesar |

### Valor de retorno

si esta fila (propiedades o datos de celdas) necesita ser procesada. false para ignorar esta fila y sus celdas y comprobar la siguiente fila.

### Ejemplos

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

### Ver también

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


