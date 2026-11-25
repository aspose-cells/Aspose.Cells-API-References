---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ConditionalFormattingIcon. Ottieni i dati del set di icone"
type: docs
url: /it/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

Ottieni i dati del set di icone

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | IconSetType | tipo dell'icona |
| indice | Int32 | indice dell'icona |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Non è necessario creare un'istanza poiché GetIconImageData è statico
            
            try
            {
                // Chiama GetIconImageData con IconSetType.Arrows3 e indice 0
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Salva i dati dell'immagine in un file per dimostrazione
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


