---
title: "FontSetting.Length"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontSetting. Obtient la longueur des caractères"
type: docs
url: /fr/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Obtient la longueur des caractères.

```csharp
public int Length { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Créer un classeur et accéder à sa première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter du texte à la cellule A1
            worksheet.Cells["A1"].PutValue("Hello World");

            // Créer des paramètres de police pour le texte de la cellule A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Démontrer l'utilisation de la propriété Length
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Modifier la longueur du paramètre de police
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Appliquer le formatage au paramètre de police
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Enregistrez le classeur
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


