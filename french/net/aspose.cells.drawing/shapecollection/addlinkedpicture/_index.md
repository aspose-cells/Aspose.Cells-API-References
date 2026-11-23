---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajouter une image liée"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Ajoute une image liée.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| hauteur | Int32 | La hauteur de la forme. En pixels |
| largeur | Int32 | La largeur de la forme. En pixels |
| sourceFullName | String | Le chemin et le nom du fichier source pour l'image liée |

### Valeur de retour

[`Picture`](../../picture/) Picture object.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte d'exemple à la cellule A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Ajouter une image liée à la feuille de calcul
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Enregistrez le classeur
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### Voir aussi

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


