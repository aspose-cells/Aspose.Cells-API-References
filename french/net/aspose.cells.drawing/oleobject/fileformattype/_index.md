---
title: "OleObject.FileFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Obtient et définit le type de fichier des données d'objet ole incorporées"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Obtient et définit le type de fichier des données d'objet ole intégré

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un objet OLE à la feuille de calcul (sans données de fichier)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Obtenir l'objet OLE ajouté
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Définir et afficher le type de format de fichier
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Enregistrez le classeur
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


