---
title: "DataSorterKey.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorterKey. Representa el tipo de clasificación"
type: docs
url: /es/net/aspose.cells/datasorterkey/type/
---
## DataSorterKey.Type property

Representa el tipo de clasificación.

```csharp
public SortOnType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyTypeDemo
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

            // Demostrar el uso de la propiedad Type
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Key Type: {key.Type}");
            }
        }
    }
}
```

### Ver también

* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


