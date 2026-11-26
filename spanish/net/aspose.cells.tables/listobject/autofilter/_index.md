---
title: "ListObject.AutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene el filtro automático de esta tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Obtiene el filtro automático de esta tabla.

```csharp
public AutoFilter AutoFilter { get; }
```

### Observaciones

Solo funciona cuando [`HasAutoFilter`](../hasautofilter/) es falso.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Crear un ListObject
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Redimensionar el objeto de lista para incluir todos los datos
            listObject.Resize(0, 0, 4, 2, true);

            // Acceder y demostrar la funcionalidad de AutoFilter
            if (listObject.AutoFilter != null)
            {
                // Aplicar filtro en la columna Edad (columna 2)
                listObject.AutoFilter.Filter(1, "25");
                
                // Mostrar datos filtrados
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Borrar el filtro
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Guarda el libro de trabajo
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


