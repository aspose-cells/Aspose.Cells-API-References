---
title: Intersect
second_title: Référence de l'API Aspose.Cells pour .NET
description: Renvoie unRangeaspose.cells/range objet qui représente lintersection rectangulaire de deux plages.
type: docs
weight: 320
url: /fr/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Renvoie un[`Range`](../../range) objet qui représente l'intersection rectangulaire de deux plages.

```csharp
public Range Intersect(Range range)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| range | Range | La plage d'intersection. |

### Return_Value

Renvoie un[`Range`](../../range) objet

### Remarques

Si les deux plages ne sont pas intersectées, renvoie null.

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
// Récupère les premières cellules de la feuille de calcul.
Cells cells = workbook.Worksheets[0].Cells;
Range range1 = cells.CreateRange("A1:A5");
Range range2 = cells.CreateRange("A3:A10");
// Récupère la plage intersectée des deux plages.
Range intersectRange = range1.Intersect(range2);
// Enregistrer le fichier Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Obtenez les premières cellules de feuille de calcul.
Dim cells as Cells = workbook.Worksheets[0].Cells
Range range1 = cells.CreateRange("A1:A5")
Range range2 = cells.CreateRange("A3:A10")
'Obtenez la plage intersectée des deux plages.
Range intersectRange = range1.Intersect(range2)
'Enregistrez le fichier Excel
workbook.Save("book1.xlsm")
```

### Voir également

* class [Range](../../range)
* espace de noms [Aspose.Cells](../../range)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
