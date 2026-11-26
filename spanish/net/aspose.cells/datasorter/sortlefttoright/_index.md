---
title: "DataSorter.SortLeftToRight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. True significa que la orientación de ordenación es de izquierda a derecha. False significa que la orientación de ordenación es de arriba a abajo. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True indica que la orientación de ordenación es de izquierda a derecha. False indica que la orientación de ordenación es de arriba a abajo. El valor predeterminado es false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo (las columnas se tratarán como filas cuando SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Crear un data sorter y configurarlo para ordenar de izquierda a derecha
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Establecer la clave de ordenación (el índice de columna se convierte en índice de fila al ordenar de izquierda a derecha)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Definir el área de ordenación (las filas se convierten en columnas al ordenar de izquierda a derecha)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Ejecuta la ordenación
            sorter.Sort(worksheet.Cells, area);

            // Guardar el resultado
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


