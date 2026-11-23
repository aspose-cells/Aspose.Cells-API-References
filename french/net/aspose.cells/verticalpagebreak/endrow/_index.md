---
title: "VerticalPageBreak.EndRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VerticalPageBreak. Obtient l'index de ligne de fin du saut de page vertical"
type: docs
url: /fr/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Obtient l'index de ligne de fin du saut de page vertical.

```csharp
public int EndRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un saut de page vertical qui couvre les lignes 3 à 8 à la colonne C (index 2)
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // Obtenir le premier saut de page vertical
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Afficher la ligne de fin du saut de page
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // Comme EndRow est en lecture seule, nous allons démontrer son obtention mais pas son réglage
            // La ligne suivante est supprimée car elle provoque une erreur de compilation :
            // vpb.EndRow = 10;
            
            // À la place, nous ajouterons un autre saut de page avec une ligne de fin différente
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


