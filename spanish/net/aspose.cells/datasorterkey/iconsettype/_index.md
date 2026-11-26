---
title: "DataSorterKey.IconSetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorterKey. Representa el tipo de conjunto de iconos"
type: docs
url: /es/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Representa el tipo de conjunto de íconos.

```csharp
public IconSetType IconSetType { get; }
```

### Observaciones

Solo tiene efecto cuando [`Type`](../type/) es Icon.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega datos de ejemplo con formato condicional de conjunto de iconos
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Agregar formato condicional de conjunto de iconos
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Crea un clasificador de datos con tipo de conjunto de iconos
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordenar los datos
            sorter.Sort(worksheet.Cells, area);

            // Muestra el tipo de conjunto de iconos de la clave del clasificador
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Guarda el libro de trabajo
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


