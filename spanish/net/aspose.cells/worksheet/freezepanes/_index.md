---
title: "Worksheet.FreezePanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Congela paneles en la celda especificada de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Congela paneles en la celda especificada de la hoja de cálculo.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| columna | Int32 | Índice de columna. |
| freezedRows | Int32 | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | Int32 | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### Observaciones

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

Los dos primeros parámetros especifican la posición congelada y los dos últimos parámetros especifican el área congelada en el panel superior izquierdo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Congelar paneles en la fila 3, columna 3, con 3 filas congeladas y 3 columnas congeladas
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Guarda el libro de trabajo
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Congela paneles en la celda especificada de la hoja de cálculo.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| freezedRows | Int32 | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | Int32 | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### Observaciones

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Congelar paneles en \"C3\" con 3 filas congeladas y 3 columnas congeladas
            worksheet.FreezePanes("C3", 3, 3);

            // Guarda el libro de trabajo
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


