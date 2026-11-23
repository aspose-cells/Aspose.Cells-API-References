---
title: "Cell.EmbeddedImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient et définit l'image intégrée dans la cellule"
type: docs
url: /fr/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Obtient et définit l'image intégrée dans la cellule.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et obtenez la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Choisir une cellule pour stocker l'image intégrée
                Cell cell = worksheet.Cells["B2"];

                // Un PNG transparent de 1x1 pixel (encodé en Base64)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Convertir la chaîne Base64 en tableau d'octets
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Définir l'image intégrée dans la cellule
                cell.EmbeddedImage = imageBytes;

                // Récupérer l'image intégrée depuis la cellule
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Écrire l'image récupérée dans un fichier pour vérifier qu'elle a été stockée correctement
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Enregistrer le classeur (l'image intégrée est stockée à l'intérieur du .xlsx)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


