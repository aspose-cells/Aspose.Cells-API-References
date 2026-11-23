---
title: "MemoryFontSource.MemoryFontSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur MemoryFontSource. Ctor"
type: docs
url: /fr/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

Constructeur.

```csharp
public MemoryFontSource(byte[] fontData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontData | Byte[] | Données de police binaires. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourceMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Charger un fichier de police TrueType dans un tableau d'octets
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // Appeler la méthode #ctor avec un paramètre tableau d'octets
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // Définir les sources de police en utilisant la classe statique FontConfigs
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // Vérifier les propriétés de la source de police
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // Utiliser la police dans une cellule
                Worksheet worksheet = workbook.Worksheets[0];
                var style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].PutValue("Text with custom font");
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error: Font file not found. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


