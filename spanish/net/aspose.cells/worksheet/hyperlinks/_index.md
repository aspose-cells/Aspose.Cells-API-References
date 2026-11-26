---
title: "Worksheet.Hyperlinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene la colección HyperlinkCollection"
type: docs
url: /es/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Obtiene la colección [`HyperlinkCollection`](../../hyperlinkcollection/).

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añada un hipervínculo a la hoja de cálculo
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Guarda el libro de trabajo
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Cargue el libro guardado para verificar el hipervínculo
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Mostrar la dirección del hipervínculo
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### Ver también

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


