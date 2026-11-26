---
title: "HorizontalPageBreakCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método HorizontalPageBreakCollection. Elimina el elemento HPageBreak en un nombre especificado"
type: docs
url: /es/net/aspose.cells/horizontalpagebreakcollection/removeat/
---
## HorizontalPageBreakCollection.RemoveAt method

Elimina el elemento HPageBreak en un nombre especificado.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | Índice del elemento, basado en cero. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            worksheet.HorizontalPageBreaks.Add(15);
            
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


