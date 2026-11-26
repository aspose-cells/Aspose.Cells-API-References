---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor CustomFilterCollection. Construye una nueva instancia"
type: docs
url: /es/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Construye una nueva instancia.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, establezca FilterColumn.FilterType como FilterType.CustomFilters y luego obtenga FilterColumn.CustomFilters. Esta propiedad será eliminada dentro de 12 meses a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
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
                // Crear una nueva CustomFilterCollection usando el constructor
                CustomFilterCollection filters = new CustomFilterCollection();

                // Mostrar el valor predeterminado de la propiedad And
                Console.WriteLine($"Default And property value: {filters.And}");

                // El constructor crea una colección vacía
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Guarda el libro de trabajo
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


