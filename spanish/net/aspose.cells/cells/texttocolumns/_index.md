---
title: "Cells.TextToColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Divide el contenido en la columna especificada en múltiples columnas"
type: docs
url: /es/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Divide el contenido en la columna especificada en múltiples columnas..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |
| totalRows | Int32 | El número de filas. |
| opciones | TxtLoadOptions | Las opciones de división. |

### Valor de retorno

Recuento total de columnas de los valores divididos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer datos de muestra con valores separados por comas
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Crear opciones de carga de texto con la coma como separador
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Dividir texto en columnas comenzando desde la celda A1, con 3 columnas de ancho
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Verifique los resultados
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


