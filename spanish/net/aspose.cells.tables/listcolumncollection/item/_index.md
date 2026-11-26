---
title: "ListColumnCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListColumnCollection. Obtiene el ListColumn por el índice"
type: docs
url: /es/net/aspose.cells.tables/listcolumncollection/item/
---
## ListColumnCollection indexer (1 of 2)

Obtiene el ListColumn por el índice.

```csharp
public ListColumn this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

el objeto ListColumn.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("T1");
            worksheet.Cells["B1"].PutValue("T2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            
            // Acceder a columnas de lista usando la propiedad Item
            ListColumn firstColumn = listObj.ListColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListColumnCollection indexer (2 of 2)

Obtiene el ListColumn por el nombre.

```csharp
public ListColumn this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre del ListColumn |

### Valor de retorno

El objeto ListColumn.

### Ver también

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


