---
title: "RangeCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método RangeCollection. Agrega un elemento Range a la colección"
type: docs
url: /es/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Agrega un [`Range`](../../range/) elemento a la colección.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | Objeto Range |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método AddRange(). Este método será eliminado 6 meses después desde diciembre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango y agregarlo a la colección
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Insertar filas para demostrar que el rango se expande
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


