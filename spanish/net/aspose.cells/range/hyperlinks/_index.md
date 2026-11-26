---
title: "Range.Hyperlinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene todos los hipervínculos en el rango"
type: docs
url: /es/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Obtiene todos los hipervínculos en el rango.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un hipervínculo a la celda A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Crear un rango que contiene A1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Obtener hipervínculos en el rango
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Mostrar información del hipervínculo
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Eliminar el hipervínculo
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Verificar que el hipervínculo haya sido eliminado
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Ver también

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


