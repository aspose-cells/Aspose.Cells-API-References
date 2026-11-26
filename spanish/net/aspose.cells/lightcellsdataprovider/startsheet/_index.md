---
title: "LightCellsDataProvider.StartSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataProvider. Inicia el guardado de una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Comienza a guardar una hoja de cálculo.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | índice de la hoja actual a guardar. |

### Valor de retorno

true si este proveedor proporcionará datos para la hoja dada; false si la hoja dada debe usar su modelo de datos normal (Cells).

### Observaciones

Se llamará al comienzo del guardado de una hoja de cálculo durante el guardado de un libro. Si el proveedor necesita referirse a

```csharp
sheetIndex
```

más tarde en el método startRow(Row) o startCell(Cell), es decir, si el proceso necesita saber qué hoja de cálculo se está procesando, la implementación debe retener el

```csharp
sheetIndex
```

value aquí.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // Crear proveedor de datos personalizado y guardar con modo de celdas ligeras
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // Se llama al iniciar el procesamiento de una hoja de cálculo
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Procesar solo la primera hoja (índice 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### Ver también

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


