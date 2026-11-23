---
title: "Style.IsLocked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non"
type: docs
url: /fr/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non.

```csharp
public bool IsLocked { get; set; }
```

### Remarques

Le verrouillage des cellules n'a aucun effet à moins que la feuille de calcul ne soit protégée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la propriété IsLocked pour une cellule
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Protéger la feuille de calcul pour appliquer le verrouillage
            worksheet.Protect(ProtectionType.All);

            // Vérifier et afficher le statut IsLocked
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Enregistrez le classeur
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


