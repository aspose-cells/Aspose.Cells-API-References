---
title: "OleObject.ObjectData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Représente les données de l'objet ole intégré sous forme de tableau d'octets"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Représente les données de l'objet ole intégré sous forme de tableau d'octets.

```csharp
public byte[] ObjectData { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            var workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            var worksheet = workbook.Worksheets[0];
            
            // Exemples de chemins de fichiers (remplacez par les chemins réels dans votre environnement)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // Ajouter un objet OLE avec des données d'image initiales
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // Modifier les données de l'objet OLE
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Enregistrez le classeur
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


