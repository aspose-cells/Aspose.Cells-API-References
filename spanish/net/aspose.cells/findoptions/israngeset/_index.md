---
title: "FindOptions.IsRangeSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Indica si el rango buscado está establecido"
type: docs
url: /es/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Indica si el rango buscado está establecido.

```csharp
public bool IsRangeSet { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // Crear una instancia de FindOptions
            FindOptions findOptions = new FindOptions();

            // Verificar el valor inicial de IsRangeSet (debe ser false)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Establecer un rango de búsqueda
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Verificar IsRangeSet después de establecer el rango (debe ser true)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Realizar una operación de búsqueda dentro del rango especificado
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Intentar encontrar algo fuera del rango (no debe encontrarse)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Guarda el libro de trabajo
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


