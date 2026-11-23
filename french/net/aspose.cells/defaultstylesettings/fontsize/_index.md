---
title: "DefaultStyleSettings.FontSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DefaultStyleSettings propriété. Obtient/Définit la taille de police standard par défaut pour le classeur"
type: docs
url: /fr/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Obtient/Définit la taille de police standard par défaut pour le classeur.

```csharp
public double FontSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Définir le nom et la taille de police par défaut
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // Charger le fichier HTML avec ces paramètres
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Accéder à une cellule et afficher sa taille de police
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### Voir aussi

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


