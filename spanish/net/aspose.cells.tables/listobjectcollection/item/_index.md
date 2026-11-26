---
title: "ListObjectCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObjectCollection. Obtiene el ListObject por índice"
type: docs
url: /es/net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Obtiene el ListObject por índice.

```csharp
public ListObject this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

El ListObject

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Acceder al objeto de lista usando la propiedad Item
            ListObject firstListObject = worksheet.ListObjects[0];
            
            // Establecer estilo de tabla
            firstListObject.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Obtiene el ListObject por nombre especificado.

```csharp
public ListObject this[string tableName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| tableName | Nombre del ListObject. |

### Valor de retorno

El ListObject

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo
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
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.DisplayName = "PersonTable";

            // Acceder al objeto de lista usando la propiedad Item por nombre
            ListObject retrievedListObj = worksheet.ListObjects["PersonTable"];
            
            // Demostrar uso convirtiendo a rango
            retrievedListObj.ConvertToRange();

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


