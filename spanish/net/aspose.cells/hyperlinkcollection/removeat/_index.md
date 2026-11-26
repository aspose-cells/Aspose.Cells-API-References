---
title: "HyperlinkCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método HyperlinkCollection. Elimina el hipervínculo en el índice especificado de esta colección"
type: docs
url: /es/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Elimina el hipervínculo en el índice especificado de esta colección.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice basado en cero del elemento. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue un hipervínculo a la celda A1
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Verificar que el hipervínculo exista antes de la eliminación
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // Elimina el hipervínculo en el índice 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // Verificar que el hipervínculo haya sido eliminado
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### Ver también

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


