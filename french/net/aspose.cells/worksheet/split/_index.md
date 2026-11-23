---
title: "Worksheet.Split"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Divise la fenêtre"
type: docs
url: /fr/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Fractionne la fenêtre.

```csharp
public void Split()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour démontrer la division
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Diviser la feuille de calcul (aucun paramètre requis)
            worksheet.Split();
            
            // Enregistrez le classeur
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


