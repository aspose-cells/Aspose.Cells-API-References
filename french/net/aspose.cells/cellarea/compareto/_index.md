---
title: "CellArea.CompareTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CellArea méthode. Comparez deux objets CellArea selon leur coin supérieur gauche"
type: docs
url: /fr/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Comparer deux objets CellArea selon leur coin supérieur gauche.

```csharp
public int CompareTo(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Valeur de retour

Si deux coins sont dans des lignes différentes, comparez alors leurs indices de ligne. Sinon comparez leurs indices de colonne. Si les deux coins sont identiques, 0 sera renvoyé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Créez deux objets CellArea pour la comparaison
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Démontrez la méthode CompareTo avec le paramètre Object
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Créez une autre comparaison avec des zones égales
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


