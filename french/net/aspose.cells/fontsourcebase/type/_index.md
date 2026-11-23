---
title: "FontSourceBase.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontSourceBase. Retourne le type de la source de police"
type: docs
url: /fr/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Renvoie le type de la source de police.

```csharp
public abstract FontSourceType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Créer une instance de classe Workbook
            Workbook workbook = new Workbook();
            
            // Créer une source de police de dossier
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Affichez la propriété Type de la source de police
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Créez une source de police à partir d'un fichier
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Affichez la propriété Type de la source de police
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Créez une source de police en mémoire (exemple avec un tableau d'octets)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Affichez la propriété Type de la source de police
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Définissez les sources de police en utilisant la méthode statique
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Enregistrez le classeur
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


