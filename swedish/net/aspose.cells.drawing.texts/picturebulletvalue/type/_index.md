---
title: "PictureBulletValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PictureBulletValue egenskap. Hämtar typen av punktens värde"
type: docs
url: /sv/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Hämtar typen av punktlistans värde.

```csharp
public override BulletType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Visa Type‑egenskapens värde (endast läs‑operation)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Demonstrera att Type är korrekt inställd på Picture för denna klass
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Spara arbetsboken
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

### Se även

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


