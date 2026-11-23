---
title: "FontConfigs.DefaultFontName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontConfigs. Obtient ou définit le nom de police par défaut"
type: docs
url: /fr/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Obtient ou définit le nom de police par défaut.

```csharp
public static string DefaultFontName { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher le nom de police par défaut actuel
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Définir un nouveau nom de police par défaut
            FontConfigs.DefaultFontName = "Arial";

            // Créer un style sans police explicite définie pour démontrer l'utilisation de la police par défaut
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Vérifier que la police a été appliquée correctement
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### Voir aussi

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


