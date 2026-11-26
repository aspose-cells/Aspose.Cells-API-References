---
title: "Cells.GetColumnWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el ancho de la columna"
type: docs
url: /es/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Obtiene el ancho de la columna.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | El índice de columna. |
| isOriginal | Booleano | Indica si se obtiene el ancho original. |
| unitType | CellsUnitType |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer el ancho de la columna 1 (índice base 0)
            cells.SetColumnWidth(0, 20);

            // Obtener el ancho de la columna en diferentes unidades y modos
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
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

## GetColumnWidth(int) {#getcolumnwidth}

Obtiene el ancho (en unidades de caracteres) de la columna especificada en vista normal

```csharp
public double GetColumnWidth(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna |

### Valor de retorno

Ancho de columna. En una hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígitos de los números 0~9 tal como se renderizan en la fuente del estilo normal.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer el ancho de la columna con índice 255
            cells.SetColumnWidth(255, 20.86);

            // Obtener y mostrar el ancho de la columna
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


