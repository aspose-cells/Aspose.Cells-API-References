---
title: "CustomFilterCollection.And"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomFilterCollection. Indica si los dos criterios tienen una relación AND"
type: docs
url: /es/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Indica si los dos criterios tienen una relación "y".

```csharp
public bool And { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Crear una nueva CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Mostrar el valor predeterminado de la propiedad And
                Console.WriteLine($"Default And property value: {filters.And}");

                // Establecer la propiedad And a true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Establecer la propiedad And a false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Guarda el libro de trabajo
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


