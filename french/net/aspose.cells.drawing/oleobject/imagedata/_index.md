---
title: "OleObject.ImageData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Représente l'image de l'objet ole sous forme de tableau d'octets"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Représente l'image de l'objet ole sous forme de tableau d'octets.

```csharp
public byte[] ImageData { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Lire le fichier image dans un tableau d'octets
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // Ajouter un objet OLE avec les données d'image
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Définir les propriétés de l'objet intégré
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // Démontrer l'utilisation de la propriété ImageData
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Enregistrez le classeur
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


