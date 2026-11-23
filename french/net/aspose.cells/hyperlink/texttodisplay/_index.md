---
title: "Hyperlink.TextToDisplay"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Hyperlink. Représente le texte à afficher pour le lien hypertexte spécifié. La valeur par défaut est l'adresse du lien hypertexte."
type: docs
url: /fr/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Représente le texte à afficher pour le lien hypertexte spécifié. La valeur par défaut est l'adresse du lien hypertexte.

```csharp
public string TextToDisplay { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyTextToDisplayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des liens hypertexte avec la propriété TextToDisplay
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Ajoutez le premier lien hypertexte avec un texte d'affichage personnalisé
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Ajouter un deuxième hyperlien avec un texte d'affichage personnalisé
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Ajouter un troisième hyperlien avec une référence de cellule comme texte d'affichage
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Enregistrez le classeur
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


