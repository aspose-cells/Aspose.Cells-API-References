---
title: "DataSorterKey.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorterKey. Obtiene el color ordenado"
type: docs
url: /es/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Obtiene el color ordenado.

```csharp
public Color Color { get; }
```

### Observaciones

Solo tiene efecto cuando [`Type`](../type/) es CellColor o FontColor.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Crea un clasificador de datos y agrega una clave
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordenar los datos
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Muestra la propiedad color de las claves
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### Ver también

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


