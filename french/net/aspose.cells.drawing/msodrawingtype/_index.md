---
title: "Énumération MsoDrawingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.MsoDrawingType. Représente le type d'objets de dessin Office"
type: docs
url: /fr/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

Représente le type d'objets de dessin Office.

```csharp
public enum MsoDrawingType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Group | `0` | Groupe |
| Line | `1` | Ligne |
| Rectangle | `2` | Rectangle |
| Oval | `3` | Ovale |
| Arc | `4` | Arc |
| Chart | `5` | Graphique |
| TextBox | `6` | Zone de texte |
| Button | `7` | Bouton |
| Picture | `8` | Image |
| Polygon | `9` | Polygone |
| CheckBox | `11` | Case à cocher |
| RadioButton | `12` | Bouton radio |
| Label | `14` | Étiquette |
| DialogBox | `15` | Boîte de dialogue |
| Spinner | `16` | Sélecteur |
| ScrollBar | `17` | Barre de défilement |
| ListBox | `18` | Boîte de liste |
| GroupBox | `19` | Boîte de groupe |
| ComboBox | `20` | Boîte combinée |
| Comment | `25` | Commentaire |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | Uniquement pour préserver l'objet de dessin dans le fichier modèle. |
| Unknown | `29` | Uniquement pour préserver l'objet de dessin dans le fichier xlsx. |
| Slicer | `31` | Segmentateur |
| WebExtension | `32` | Extension Web |
| SmartArt | `33` | Smart Art |
| CustomXml | `34` | Forme xml personnalisée, telle que Ink. |
| Timeline | `35` | Chronologie |
| Model3D | `36` | Modèle 3D |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoDrawingTypeDemo
    {
        public static void MsoDrawingTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle à la feuille de calcul
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // Ajouter une forme ovale à la feuille de calcul
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // Ajouter une forme de ligne à la feuille de calcul
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // Ajouter une forme de zone de texte à la feuille de calcul
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // Afficher les noms et les types des formes
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // Enregistrez le classeur
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


