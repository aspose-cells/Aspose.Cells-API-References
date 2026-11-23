---
title: "Font.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit la couleur de la police"
type: docs
url: /fr/net/aspose.cells/font/color/
---
## Font.Color property

Obtient ou définit la couleur de la police.

```csharp
public Color Color { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le HTML avec différentes couleurs et styles de police
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Obtenir le formatage de texte enrichi
            FontSetting[] richText = cell.GetCharacters();
            
            // Vérifier et démontrer les propriétés de couleur
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Enregistrez le classeur
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


