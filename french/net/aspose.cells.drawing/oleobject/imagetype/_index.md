---
title: "OleObject.ImageType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Obtient le format d'image de l'objet ole"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

Obtient le format d'image de l'objet ole.

```csharp
public ImageType ImageType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE à la feuille de calcul
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Afficher le type d'image actuel de l'objet OLE
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // Démontrer comment utiliser la propriété ImageType
            if (oleObject.ImageType == ImageType.Unknown)
            {
                Console.WriteLine("The OLE object's image format is not recognized.");
            }
            else if (oleObject.ImageType == ImageType.Emf)
            {
                Console.WriteLine("The OLE object uses EMF image format.");
            }
            else if (oleObject.ImageType == ImageType.Png)
            {
                Console.WriteLine("The OLE object uses PNG image format.");
            }

            // Enregistrez le classeur
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


