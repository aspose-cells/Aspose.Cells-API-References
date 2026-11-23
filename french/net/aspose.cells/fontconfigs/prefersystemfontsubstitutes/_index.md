---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontConfigs. Indique s'il faut d'abord utiliser les substituts de police système ou non lorsqu'une police n'est pas présentée et que le substitut de cette police n'est pas défini. par ex. Sous Ubuntu la police Arial est généralement substituée par Liberation Sans. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Indique s'il faut d'abord utiliser les substituts de police du système ou non lorsqu'une police n'est pas disponible et que le substitut de cette police n'est pas défini. Par exemple, sous Ubuntu, la police "Arial" est généralement substituée par "Liberation Sans". La valeur par défaut est false.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher la valeur actuelle de PreferSystemFontSubstitutes
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // Définir PreferSystemFontSubstitutes sur true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // Créer une cellule avec une police qui pourrait nécessiter une substitution
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Enregistrer le classeur pour voir les effets de substitution de police
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Réinitialiser à la valeur par défaut
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### Voir aussi

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


