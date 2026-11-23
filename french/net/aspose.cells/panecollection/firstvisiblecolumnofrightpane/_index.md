---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaneCollection. Obtient et définit la première colonne visible du volet droit"
type: docs
url: /fr/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Obtient et définit la première colonne visible du volet droit.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Figer les volets en spécifiant les indices de ligne et de colonne (5, 3)
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Obtenir la collection de volets
            PaneCollection panes = sheet.GetPanes();
            
            // Définir la première colonne visible du volet droit
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


