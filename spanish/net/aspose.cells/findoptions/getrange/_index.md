---
title: "FindOptions.GetRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FindOptions. Obtiene y establece el rango buscado"
type: docs
url: /es/net/aspose.cells/findoptions/getrange/
---
## FindOptions.GetRange method

Obtiene y establece el rango buscado.

```csharp
public CellArea GetRange()
```

### Valor de retorno

Devuelve el rango buscado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsMethodGetRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue("Grape");
            worksheet.Cells["B3"].PutValue("Lemon");

            // Crear una instancia de FindOptions
            FindOptions findOptions = new FindOptions();
            findOptions.LookInType = LookInType.Values;
            findOptions.LookAtType = LookAtType.Contains;

            // Establecer el rango de búsqueda a A1:B3
            CellArea searchArea = new CellArea();
            searchArea.StartRow = 0;
            searchArea.StartColumn = 0;
            searchArea.EndRow = 2;
            searchArea.EndColumn = 1;
            findOptions.SetRange(searchArea);

            try
            {
                // Obtener el rango que se estableció
                CellArea resultRange = findOptions.GetRange();

                // Mostrar la información del rango
                Console.WriteLine($"Search range: StartRow={resultRange.StartRow}, StartColumn={resultRange.StartColumn}, " +
                    $"EndRow={resultRange.EndRow}, EndColumn={resultRange.EndColumn}");

                // Realizar una operación de búsqueda para demostrar que se está usando el rango
                Cell foundCell = worksheet.Cells.Find("an", null, findOptions);
                if (foundCell != null)
                {
                    Console.WriteLine($"Found value '{foundCell.StringValue}' at {foundCell.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodGetRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


