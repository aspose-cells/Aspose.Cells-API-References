---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DefaultStyleSettings. Obtient/Définit la valeur par défaut pour l'alignement vertical"
type: docs
url: /fr/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Obtient/Définit la valeur par défaut pour l'alignement vertical

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir l'alignement vertical par défaut sur Bas
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Vérifier que l'alignement vertical est appliqué à toutes les cellules
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Enregistrez le classeur
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


