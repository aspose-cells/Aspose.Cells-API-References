---
title: "Worksheet.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet property. Représente le type de feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Représente le type de feuille de calcul.

```csharp
public SheetType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir quelques propriétés de base
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Ajouter une feuille de graphique pour démontrer différents types de feuille de calcul
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Comparer les types de feuilles de calcul
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Enregistrez le classeur
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


