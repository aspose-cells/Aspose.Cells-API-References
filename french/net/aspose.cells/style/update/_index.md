---
title: "Style.Update"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Applique le style nommé aux styles des cellules qui utilisent ce style nommé. Cela fonctionne comme cliquer sur le bouton OK après avoir terminé la modification du style. S'applique uniquement aux styles nommés"
type: docs
url: /fr/net/aspose.cells/style/update/
---
## Style.Update method

Applique le style nommé aux styles des cellules qui utilisent ce style nommé. Cela fonctionne comme en cliquant sur le bouton "ok" après avoir terminé la modification du style. S'applique uniquement au style nommé.

```csharp
public void Update()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Appliquer le style à la cellule A1
            worksheet.Cells["A1"].SetStyle(style);
            
            // Modifier le style
            style.Number = 4; // Change to Currency format
            
            // Mettre à jour les modifications du style
            style.Update();
            
            // Vérifier que le style a été mis à jour
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


