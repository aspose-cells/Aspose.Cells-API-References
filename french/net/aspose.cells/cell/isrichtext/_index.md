---
title: "Cell.IsRichText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Indique si la valeur chaîne de cette cellule est un texte riche formaté"
type: docs
url: /fr/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indique si la valeur chaîne de cette cellule est un texte formaté richement.

```csharp
public bool IsRichText()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une cellule avec un formatage de texte riche
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Appliquer le formatage de texte riche
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Vérifier si la cellule contient du texte riche
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Enregistrez le classeur
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


