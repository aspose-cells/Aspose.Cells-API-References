---
title: "ListColumn.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListColumn. Obtiene y establece el nombre de la columna"
type: docs
url: /es/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Obtiene y establece el nombre de la columna.

```csharp
public string Name { get; set; }
```

### Observaciones

Si se establece el nombre de la columna, el valor de la celda correspondiente también se cambiará.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Crear un objeto tabla/lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // Acceda y modifique la propiedad Name de la primera columna de lista
            listObject.ListColumns[0].Name = "NewID";
            
            // Verificar que el nombre se haya establecido
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Guarda el libro de trabajo
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


