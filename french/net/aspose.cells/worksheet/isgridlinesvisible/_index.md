---
title: "Worksheet.IsGridlinesVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient ou définit une valeur indiquant si les quadrillages sont visibles. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Obtient ou définit une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la visibilité des quadrillages sur true
            worksheet.IsGridlinesVisible = true;
            
            // Ajouter des données d'exemple pour voir les lignes de grille
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Ajuster automatiquement les colonnes pour une meilleure visibilité
            worksheet.AutoFitColumns();
            
            // Enregistrez le classeur
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


