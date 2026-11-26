---
title: "ProtectedRangeCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ProtectedRangeCollection. Obtiene el elemento ProtectedRange en el índice especificado"
type: docs
url: /es/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Obtiene el elemento [`ProtectedRange`](../../protectedrange/) en el índice especificado.

```csharp
public ProtectedRange this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añadir un rango protegido usando índices de celda (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Acceder al rango protegido usando la propiedad Item (índice 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Verificar y mostrar el estado de protección
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


