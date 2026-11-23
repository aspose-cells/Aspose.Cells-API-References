---
title: "FontSetting.FontSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur FontSetting."
type: docs
url: /fr/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 |  |
| longueur | Int32 |  |
| feuilles | WorksheetCollection |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte d'exemple à la cellule
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Créer un paramètre de police pour les 5 premiers caractères (0-4) dans toutes les feuilles de calcul
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Appliquer la mise en forme
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


