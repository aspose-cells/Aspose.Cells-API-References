---
title: "DefaultStyleSettings.FontName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DefaultStyleSettings propriété. Obtient/Définit le nom de police par défaut pour le classeur"
type: docs
url: /fr/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Obtient/Définit le nom de police par défaut pour le classeur

```csharp
public string FontName { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Créer des options de chargement et définir le nom de police
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Créer un nouveau classeur avec les options de chargement
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Accéder au style par défaut et vérifier le nom de police
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Créer une feuille de calcul et définir la valeur de la cellule
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Enregistrez le classeur
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### Voir aussi

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


