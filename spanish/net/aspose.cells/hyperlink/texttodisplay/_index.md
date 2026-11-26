---
title: "Hyperlink.TextToDisplay"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Hyperlink. Representa el texto que se mostrará para el hipervínculo especificado. El valor predeterminado es la dirección del hipervínculo"
type: docs
url: /es/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Representa el texto que se mostrará para el hipervínculo especificado. El valor predeterminado es la dirección del hipervínculo.

```csharp
public string TextToDisplay { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyTextToDisplayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar hipervínculos con la propiedad TextToDisplay
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Agregar el primer hipervínculo con texto de visualización personalizado
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Agregar segundo hipervínculo con texto de visualización personalizado
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Agregar tercer hipervínculo con referencia de celda como texto de visualización
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Guarda el libro de trabajo
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### Ver también

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


