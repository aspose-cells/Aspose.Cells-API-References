---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PasteOptions. Ignorar enlaces al archivo original"
type: docs
url: /es/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ignorar enlaces al archivo original.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Crear datos de muestra con fórmulas que podrían enlazar al archivo original
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Crear hoja de cálculo de destino y rango
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Configurar opciones de pegado para ignorar enlaces al archivo original
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Copiar con las opciones de pegado especificadas
            dstRange.Copy(srcRange, pasteOptions);

            // Guarda el libro de trabajo
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


