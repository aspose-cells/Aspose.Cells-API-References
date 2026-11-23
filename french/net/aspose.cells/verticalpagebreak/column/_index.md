---
title: "VerticalPageBreak.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VerticalPageBreak. Obtient l'index de colonne du saut de page vertical"
type: docs
url: /fr/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Obtient l'index de colonne du saut de page vertical.

```csharp
public int Column { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des sauts de page verticaux aux colonnes 4 et 8
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Obtenir la collection des sauts de page verticaux
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Afficher les informations sur chaque saut de page vertical
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Enregistrez le classeur
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


