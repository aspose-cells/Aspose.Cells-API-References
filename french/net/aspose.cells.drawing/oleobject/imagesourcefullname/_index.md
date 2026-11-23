---
title: "OleObject.ImageSourceFullName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Obtient ou définit le chemin et le nom du fichier source pour l'image liée"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Obtient ou définit le chemin et le nom du fichier source pour l'image liée.

```csharp
public string ImageSourceFullName { get; set; }
```

### Remarques

La valeur par défaut est une chaîne vide. Si SourceFullName n'est pas une chaîne vide, l'image est liée. Si SourceFullName n'est pas une chaîne vide, mais que Data est nul, alors l'image est liée et n'est pas stockée dans le fichier.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fichier PDF d'exemple à intégrer
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Ajouter un OleObject à la feuille de calcul
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // Définir les propriétés OleObject incluant ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Enregistrez le classeur
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


