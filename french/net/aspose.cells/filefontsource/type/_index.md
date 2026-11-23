---
title: "FileFontSource.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FileFontSource. Retourne le type de la source de police"
type: docs
url: /fr/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Renvoie le type de la source de police.

```csharp
public override FontSourceType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string fontFilePath = "CustomFont.ttf";
            
            // Créer une instance de FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Créer le classeur et appliquer la police
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Text with custom font");
            
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);
            
            workbook.Save("FontSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


