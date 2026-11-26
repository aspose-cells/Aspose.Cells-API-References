---
title: "ListObject.HasAutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Indica si se aplica filtro automático a esta tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Indica si el filtro automático se aplica a esta tabla.

```csharp
public bool HasAutoFilter { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo para la tabla
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Agregar un ListObject (tabla) que cubra el rango de datos
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Asegurar que la tabla se redimensione para incluir todas las filas
                listObject.Resize(0, 0, 4, 2, true);

                // Leer y mostrar el valor de la propiedad HasAutoFilter
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // El objeto AutoFilter se puede acceder a través de la propiedad AutoFilter
                // Demostrar que no es nulo cuando HasAutoFilter es verdadero
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Aplicar un filtro simple en la columna "Score" (índice 1) para mostrar filas con Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Usar Cells.Rows para comprobar si la fila está oculta
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Borrar el filtro
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Guardar el libro de trabajo (opcional)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


