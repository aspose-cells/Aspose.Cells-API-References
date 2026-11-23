---
title: "Picture.SourceFullName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Picture. Obtient ou définit le chemin et le nom du fichier source pour l'image liée"
type: docs
url: /fr/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Obtient ou définit le chemin et le nom du fichier source pour l'image liée.

```csharp
public string SourceFullName { get; set; }
```

### Remarques

La valeur par défaut est une chaîne vide. Si SourceFullName n'est pas une chaîne vide, l'image est liée. Si SourceFullName n'est pas une chaîne vide, mais que Data est nul, alors l'image est liée et n'est pas stockée dans le fichier.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image liée à la feuille de calcul
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // Démontrer la propriété SourceFullName
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


