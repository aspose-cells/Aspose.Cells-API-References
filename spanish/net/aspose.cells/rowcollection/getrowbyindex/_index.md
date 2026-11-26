---
title: "RowCollection.GetRowByIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método RowCollection. Obtiene el objeto fila por la posición en la lista"
type: docs
url: /es/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Obtiene el objeto fila por la posición en la lista.

```csharp
public Row GetRowByIndex(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | La posición. |

### Valor de retorno

El objeto Row en la posición dada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtener fila por índice (base 0)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### Ver también

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


