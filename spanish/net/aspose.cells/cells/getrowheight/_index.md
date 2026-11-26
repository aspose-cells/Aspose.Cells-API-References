---
title: "Cells.GetRowHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura de las filas"
type: docs
url: /es/net/aspose.cells/cells/getrowheight/
---
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}

Obtiene la altura de la fila.

```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| isOriginal | Booleano | Indica si devuelve la altura original de la fila o 0 para una fila oculta. |
| unitType | CellsUnitType | Tipo de unidad del valor de altura devuelto |

### Valor de retorno

Altura de la fila

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la altura de la fila para la fila 3 (20 píxeles)
            worksheet.Cells.SetRowHeightPixel(3, 20);
            
            // Obtener la altura de la fila en diferentes unidades
            double heightInPixels = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Pixel);
            double heightInPoints = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Point);
            
            // Genere la salida de los resultados
            Console.WriteLine("Row height in pixels: " + heightInPixels);
            Console.WriteLine("Row height in points: " + heightInPoints);
        }
    }
}
```

### Ver también

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRowHeight(int) {#getrowheight}

Obtiene la altura de una fila especificada, en unidades de puntos.

```csharp
public double GetRowHeight(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |

### Valor de retorno

Altura de la fila

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets["Sheet1"];
            Cells cells = ws.Cells;
            
            string strText = "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.";
            cells[0, 0].PutValue(strText);
            
            Style style = cells[0, 0].GetStyle();
            style.IsTextWrapped = true;
            cells[0, 0].SetStyle(style);
            
            ws.Cells.SetColumnWidth(0, 50);
            ws.AutoFitRows();
            
            double rowHeight = cells.GetRowHeight(0);
            Console.WriteLine("Row height: " + rowHeight);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


