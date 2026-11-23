---
title: "LineFormat.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LineFormat. Détermine si cette instance a la même valeur qu'un autre objet LineFormat spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Détermine si cette instance a la même valeur qu'un autre objet [`LineFormat`](../) spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | L'objet [`LineFormat`](../) à comparer avec cette instance. |

### Valeur de retour

true si la valeur du paramètre obj est identique à la valeur de cette instance ; sinon, false. Si obj est null, cette méthode renvoie false.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme de ligne à la feuille de calcul
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // Obtenez le format de ligne de la première forme
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Comparez les formats de ligne en utilisant la méthode Equals
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### Voir aussi

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


