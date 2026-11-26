---
title: "ExternalLinkCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLinkCollection. Obtiene el elemento ExternalLink en el índice especificado"
type: docs
url: /es/net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

Obtiene el elemento [`ExternalLink`](../../externallink/) en el índice especificado.

```csharp
public ExternalLink this[int index] { get; }
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
    public class ExternalLinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con enlaces externos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos enlaces externos
            worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
            worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
            
            // Acceda a los enlaces externos usando la propiedad Item
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                ExternalLink link = workbook.Worksheets.ExternalLinks[i];
                Console.WriteLine($"External Link {i + 1}:");
                Console.WriteLine($"- DataSource: {link.DataSource}");
                Console.WriteLine($"- OriginalDataSource: {link.OriginalDataSource}");
            }
        }
    }
}
```

### Ver también

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


