---
title: "Clase BorderCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.BorderCollection. Encapsula una colección de objetos Border"
type: docs
url: /es/net/aspose.cells/bordercollection/
---
## BorderCollection class

Encapsula una colección de objetos [`Border`](../border/).

```csharp
public class BorderCollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Obtiene o establece el Color de las líneas diagonales. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Obtiene o establece el estilo de las líneas diagonales. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Indica si los bordes izquierdo, derecho, superior e inferior deben aplicarse solo a los bordes externos de un rango de celdas. El valor predeterminado es true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Obtiene el elemento [`Border`](../border/) en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Establece el Color de todos los bordes en la colección. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Establece el estilo de todos los bordes de la colección. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Añadiendo una nueva hoja de cálculo al objeto Workbook
            workbook.Worksheets.Add();

            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];

            // Accediendo a la celda "A1" de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];

            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Visit Aspose!");

            // Obteniendo el estilo de la celda
            Style style = cell.GetStyle();

            // Estableciendo el estilo de línea del borde superior
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Estableciendo el color del borde superior
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Estableciendo el estilo de línea del borde inferior
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Estableciendo el color del borde inferior
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Estableciendo el estilo de línea del borde izquierdo
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Estableciendo el color del borde izquierdo
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Estableciendo el estilo de línea del borde derecho
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Estableciendo el color del borde derecho
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Estableciendo propiedades diagonales
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Aplicando el estilo a la celda
            cell.SetStyle(style);

            // Guardando el archivo Excel
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


