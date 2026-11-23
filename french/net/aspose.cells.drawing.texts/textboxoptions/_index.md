---
title: "Class TextBoxOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.TextBoxOptions. Représente les options de texte de la forme"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Représente les options de texte de la forme

```csharp
public class TextBoxOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Autoriser le texte à dépasser la forme. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Renvoie la marge inférieure en unités de points |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Obtient et définit la marge gauche en unité de Points. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Indique s'il faut redimensionner la forme pour ajuster le texte |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Obtient et définit la marge droite en unité de Points. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Obtient ou définit la direction d'affichage du texte dans un corps de texte donné. Cela correspond à "Format Shape - Text Options - Text Box - Text direction" dans Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Il correspond à "Format Shape - Text Options - Text Box - Vertical Alignment" dans Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Obtient et définit la marge supérieure en unité de Points. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Spécifie le retour à la ligne du texte dans une forme. False - Aucun retour à la ligne ne se produira dans le corps du texte. True - Le retour à la ligne se produira dans le corps du texte. |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//faites votre travail

//Enregistrer le fichier Excel.
workbook.Save("exmaple.xlsx");
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


