---
title: "DataSorter.Order1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DataSorter property. Representa el orden de clasificación de la primera clave"
type: docs
url: /es/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Representa el orden de clasificación de la primera clave.

```csharp
public SortOrder Order1 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Establecer propiedades del ordenamiento de datos
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Definir rango de ordenación
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Ejecuta la ordenación
            sorter.Sort(worksheet.Cells, area);
            
            // Guarda el libro de trabajo
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### Ver también

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


