---
title: "PictureBulletValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PictureBulletValue. Ottiene il tipo del valore del bullet"
type: docs
url: /it/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Ottiene il tipo del valore del punto elenco.

```csharp
public override BulletType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class PictureBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un'istanza di PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Visualizza il valore della proprietà Type (operazione di sola lettura)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Dimostra che la proprietà Type è correttamente impostata su Picture per questa classe
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("PictureBulletValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


