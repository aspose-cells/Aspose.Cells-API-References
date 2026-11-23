---
title: "PictureBulletValue.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PictureBulletValue. Obtient le type de la valeur de la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Obtient le type de la valeur de la puce.

```csharp
public override BulletType Type { get; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une instance de PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Affichez la valeur de la propriété Type (opération en lecture seule)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Démontrez que le Type est correctement défini sur Picture pour cette classe
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Enregistrez le classeur
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

### Voir aussi

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


