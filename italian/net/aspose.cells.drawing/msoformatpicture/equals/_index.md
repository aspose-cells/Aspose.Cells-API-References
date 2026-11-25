---
title: "MsoFormatPicture.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo MsoFormatPicture."
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/equals/
---
## MsoFormatPicture.Equals method

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPictureMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi due immagini al foglio di lavoro
            int pictureIndex1 = worksheet.Pictures.Add(0, 0, "example.jpg");
            int pictureIndex2 = worksheet.Pictures.Add(5, 0, "example.jpg");
            
            Picture picture1 = worksheet.Pictures[pictureIndex1];
            Picture picture2 = worksheet.Pictures[pictureIndex2];

            // Ottieni gli oggetti MsoFormatPicture
            MsoFormatPicture format1 = picture1.FormatPicture;
            MsoFormatPicture format2 = picture2.FormatPicture;

            // Imposta proprietà diverse per dimostrare il confronto di uguaglianza
            format1.Brightness = 0.5;
            format1.Contrast = 0.3;
            format2.Brightness = 0.5;
            format2.Contrast = 0.3;

            try
            {
                // Confronta i due oggetti MsoFormatPicture
                bool areEqual = format1.Equals((object)format2);
                Console.WriteLine($"Format objects are equal: {areEqual}");

                // Modifica un formato e confronta di nuovo
                format2.Brightness = 0.7;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, format objects are equal: {areEqual}");

                // Confronta con null
                bool isNullEqual = format1.Equals((object)null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Confronta con un tipo diverso
                bool isDifferentTypeEqual = format1.Equals((object)"string");
                Console.WriteLine($"Comparison with different type: {isDifferentTypeEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MsoFormatPictureMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


