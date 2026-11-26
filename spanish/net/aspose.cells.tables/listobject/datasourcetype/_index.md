---
title: "ListObject.DataSourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene el tipo de origen de datos de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/datasourcetype/
---
## ListObject.DataSourceType property

Obtiene el tipo de origen de datos de la tabla.

```csharp
public TableDataSourceType DataSourceType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataSourceTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Crear objeto de lista y obtenerlo de la colección
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            listObject.DisplayName = "EmployeeTable";

            // Obtener y mostrar DataSourceType
            TableDataSourceType dataSourceType = listObject.DataSourceType;
            Console.WriteLine("ListObject DataSourceType: " + dataSourceType);

            workbook.Save("ListObjectDataSourceTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


