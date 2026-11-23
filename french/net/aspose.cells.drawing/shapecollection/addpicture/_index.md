---
title: "ShapeCollection.AddPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une image à la collection"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addpicture/
---
## AddPicture(int, int, int, int, Stream) {#addpicture}

Ajoute une image à la collection.

```csharp
public Picture AddPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| bottomRow | Int32 | Index de la ligne du coin inférieur droit |
| rightColumn | Int32 | Index de la colonne du coin inférieur droit |
| stream | Stream | Objet Stream qui contient les données de l'image. |

### Valeur de retour

[`Picture`](../../picture/) Picture object.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddPictureWithInt32Int32Int32Int32StreamDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajoutez une image à partir d'un flux de fichier
            using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
            {
                Picture picture = shapes.AddPicture(1, 0, 1, 0, fs);
            }

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddPicture(int, int, Stream, int, int) {#addpicture_1}

Ajoute une image à la collection.

```csharp
public Picture AddPicture(int topRow, int leftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| stream | Stream | Objet Stream qui contient les données de l'image. |
| widthScale | Int32 | Échelle de la largeur de l'image, en pourcentage. |
| heightScale | Int32 | Échelle de la hauteur de l'image, en pourcentage. |

### Valeur de retour

[`Picture`](../../picture/) Picture object.

### Exemples

```csharp

[C#]
//ajouter une image
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    Picture picture = shapes.AddPicture(1, 1, fs, 50, 60);
}
```

### Voir aussi

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


