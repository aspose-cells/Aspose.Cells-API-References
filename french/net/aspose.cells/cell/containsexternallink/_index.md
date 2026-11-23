---
title: "Cell.ContainsExternalLink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule"
type: docs
url: /fr/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule.

```csharp
public bool ContainsExternalLink { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple et un lien externe
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Vérifiez si les cellules contiennent des liens externes
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


