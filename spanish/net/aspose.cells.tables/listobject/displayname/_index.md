---
title: "ListObject.DisplayName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene y establece el nombre para mostrar de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Obtiene y establece el nombre para mostrar de la tabla.

```csharp
public string DisplayName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Establecer el nombre para mostrar y demostrar su uso
            listObject.DisplayName = "ProductTable";
            Console.WriteLine("List Object Display Name: " + listObject.DisplayName);

            // Guarda el libro de trabajo
            workbook.Save("ListObjectDisplayNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


