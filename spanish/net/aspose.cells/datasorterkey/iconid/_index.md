---
title: "DataSorterKey.IconId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorterKey. Representa el id del tipo de conjunto de iconos"
type: docs
url: /es/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Representa el id del tipo de conjunto de íconos.

```csharp
public int IconId { get; }
```

### Observaciones

Solo tiene efecto cuando [`Type`](../type/) es Icon.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega datos de ejemplo con valores que podrían usar conjuntos de iconos
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

            // Crea un clasificador de datos y agrega una clave
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordenar los datos
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Muestra la propiedad IconId de las claves del clasificador
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Guarda el libro de trabajo
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


