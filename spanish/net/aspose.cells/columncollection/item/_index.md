---
title: "ColumnCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColumnCollection. Obtiene un objeto Column por índice de columna. El objeto Column del índice de columna dado se instanciará si no existe previamente"
type: docs
url: /es/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Obtiene un objeto [`Column`](../../column/) por índice de columna. El objeto Column del índice de columna dado se instanciará si no existe previamente.

```csharp
public Column this[int columnIndex] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de columnas
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Establecer el ancho de las columnas usando la propiedad Item
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Mostrar los anchos de columna
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Verificar que los anchos de columna estén configurados correctamente
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### Ver también

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


