---
title: "DataSorter.AddColorKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DataSorter. Añade una clave de ordenación por color"
type: docs
url: /es/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Agrega una clave de ordenación por color.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | Int32 | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| type | SortOnType | El tipo de valor de color ordenado. |
| orden | SortOrder | El orden de clasificación. |
| color | Color | El color de ordenación personalizado. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con celdas coloreadas
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Aplicar colores a las celdas
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Crear ordenador de datos y agregar clave de color
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Ordenar los datos
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Salida de los valores ordenados (para demostración)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### Ver también

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


