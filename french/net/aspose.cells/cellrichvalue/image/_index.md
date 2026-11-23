---
title: "CellRichValue.Image"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellRichValue. Obtient les données d'image de la cellule"
type: docs
url: /fr/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Obtient les données d'image de la cellule.

```csharp
public virtual byte[] Image { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Obtenir la cell rich value contenant l'image
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Accéder à la valeur enrichie
            CellRichValue richValue = cell.GetRichValue();

            // Afficher les propriétés de l'image
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Définir un nouveau texte alternatif pour l'image
            richValue.AltText = "Sample product image";

            // Enregistrez le classeur
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


