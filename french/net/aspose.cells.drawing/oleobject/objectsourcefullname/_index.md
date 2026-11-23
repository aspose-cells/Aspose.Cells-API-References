---
title: "OleObject.ObjectSourceFullName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Retourne le nom complet de la source du fichier source pour l'objet OLE lié"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Renvoie le nom complet source du fichier source pour l'objet OLE lié.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Remarques

Ne prend en charge la définition du nom complet de la source que lorsque le type de fichier est OleFileType.Unknown. Par exemple les fichiers wav, avi, etc.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE (en utilisant les données du fichier sous forme de tableau d'octets)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Définir et obtenir ObjectSourceFullName
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

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


