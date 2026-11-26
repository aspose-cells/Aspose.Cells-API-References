---
title: "ListObject.Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListObject. Filtrar la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/filter/
---
## ListObject.Filter method

Filtrar la tabla.

```csharp
[Obsolete("Use set ListObject.HasAutoFilter property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter Filter()
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor establezca la propiedad ListObject.HasAutoFilter./// Esta propiedad será eliminada 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectMethodFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo para el objeto de lista
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Smartphone");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Monitor");
            worksheet.Cells["B4"].PutValue(250);

            try
            {
                // Crear un objeto de lista a partir de un rango de datos usando ListObjects.Add con los parámetros correctos
                int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[listObjectIndex];
                
                // Obtener AutoFilter mediante el método Filter
                AutoFilter autoFilter = listObject.Filter();

                // Aplicar filtro en la columna Price (índice 1) para mostrar los elementos >= 800
                autoFilter.Custom(1, FilterOperatorType.GreaterOrEqual, 800);

                Console.WriteLine("Filter applied successfully. Showing items with Price >= 800.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Filter method: {ex.Message}");
            }

            workbook.Save("ListObjectMethodFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


