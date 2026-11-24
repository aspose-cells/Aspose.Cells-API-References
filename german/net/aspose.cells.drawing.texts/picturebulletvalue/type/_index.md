---
title: "PictureBulletValue.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PictureBulletValue-Eigenschaft. Liest den Typ des Aufzählungswerts"
type: docs
url: /de/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Ermittelt den Typ des Aufzählungszeichenwerts.

```csharp
public override BulletType Type { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine Instanz von PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Zeige den Wert der Type-Eigenschaft an (nur lesende Operation)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Demonstriere, dass der Type für diese Klasse korrekt auf Picture gesetzt ist
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


