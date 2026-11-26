---
title: "LightCellsDataHandler.StartSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataHandler. Inicia el procesamiento de una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

Comienza a procesar una hoja de cálculo.

```csharp
public bool StartSheet(Worksheet sheet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hoja | Hoja de cálculo | la hoja de cálculo para leer los datos de celdas. |

### Valor de retorno

si los datos de celdas de esta hoja necesitan ser procesados. false para ignorar esta hoja.

### Observaciones

Se llamará antes de leer los datos de celdas de una hoja de cálculo.

### Ejemplos

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

### Ver también

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


