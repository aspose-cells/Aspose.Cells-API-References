---
title: "LoadOptions.StandardFontSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Définit la taille de police standard par défaut"
type: docs
url: /fr/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Définit la taille de police standard par défaut.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser DefaultStyleSettings. Cette propriété sera supprimée 12 mois plus tard à compter de mars 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // Créez des options de chargement HTML et définissez StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // Chargez le classeur avec les options
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Accéder à la première feuille de calcul et aux cellules
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Définissez un texte d'exemple et vérifiez les propriétés de police
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


