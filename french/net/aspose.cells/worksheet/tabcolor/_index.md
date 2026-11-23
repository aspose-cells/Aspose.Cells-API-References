---
title: "Worksheet.TabColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente la couleur d'onglet de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Représente la couleur de l'onglet de la feuille de calcul.

```csharp
public Color TabColor { get; set; }
```

### Remarques

Cette fonctionnalité n'est prise en charge que dans ExcelXP (Excel2002) et les versions ultérieures. Si vous enregistrez le fichier au format Excel97 ou Excel2000, elle sera omise.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la couleur d'onglet sur rouge
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Effacer la couleur d'onglet
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Enregistrer le classeur modifié
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


