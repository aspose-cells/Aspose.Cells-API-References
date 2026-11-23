---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un objet équation à la feuille de calcul en utilisant des chaînes de format LaTeX"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Ajoute un objet équation à la feuille de calcul en utilisant des chaînes au format LaTeX.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | L'index de la ligne supérieure. |
| haut | Int32 | Le décalage vertical de sa ligne supérieure, en pixels. |
| leftColumn | Int32 | L'index de la colonne de gauche. |
| gauche | Int32 | Le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | La hauteur de l'équation, en unité de pixel. |
| largeur | Int32 | La largeur de l'équation, en unité de pixel. |
| latex | String | Chaîne de format LaTeX |

### Exemples

```csharp

[C#]
// Chaîne de format LaTeX.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Ajoute un objet équation à la feuille de calcul.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### Voir aussi

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


