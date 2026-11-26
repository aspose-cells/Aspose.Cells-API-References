---
title: "Cells.GetFirstDataRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el índice de la primera fila de la celda que contiene datos en la columna especificada"
type: docs
url: /es/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Obtiene el índice de la primera fila de la celda que contiene datos en la columna especificada.

```csharp
public int GetFirstDataRow(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |

### Valor de retorno

índice de la primera fila.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo para demostrar el método
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Obtener la colección Cells de la hoja de cálculo
                Cells cells = worksheet.Cells;

                // Llamar a GetFirstDataRow para la columna A (índice 0)
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Llamar a GetFirstDataRow para la columna B (índice 1)
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Llamar a GetFirstDataRow para la columna C (índice 2)
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Guarda el libro de trabajo
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


