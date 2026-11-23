---
title: "StyleFlag.Locked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre Verrouillé sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Le paramètre verrouillé sera appliqué.

```csharp
public bool Locked { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un style et définir sa propriété locked
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Créer un style flag et activer le flag locked
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Appliquer le style à la cellule A1
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Vérifier le statut locked
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Protéger la feuille de calcul pour voir l'effet de verrouillage
            worksheet.Protect(ProtectionType.All);

            // Essayer de modifier la cellule locked (générera une exception lorsque la feuille de calcul est protégée)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


