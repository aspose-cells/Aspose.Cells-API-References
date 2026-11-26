---
title: "Hyperlink.Delete"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Hyperlink. Elimina este hipervínculo"
type: docs
url: /es/net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Elimina este hipervínculo

```csharp
public void Delete()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkMethodDeleteDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos hipervínculos para demostrar la eliminación
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
            
            Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
            
            // Eliminar todos los hipervínculos
            for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
            {
                worksheet.Hyperlinks[i].Delete();
            }
            
            Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Ver también

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


