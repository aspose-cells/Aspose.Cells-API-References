---
title: "OleObject.FullObjectBin"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "OleObject propriété. Obtient les données binaires complètes de l'objet OLE intégré dans le fichier modèle"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/fullobjectbin/
---
## OleObject.FullObjectBin property

Obtient les données binaires complètes de l'objet ole intégré dans le fichier modèle.

```csharp
public byte[] FullObjectBin { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyFullObjectBinDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE à la feuille de calcul
            byte[] objectData = File.ReadAllBytes("example.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, objectData, "docx");
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Définir certaines propriétés pour l'objet OLE
            oleObject.FileFormatType = FileFormatType.Docx;
            oleObject.ObjectData = objectData;
            oleObject.IsAutoSize = true;

            // Obtenir les données FullObjectBin (propriété en lecture seule)
            byte[] fullObjectBinData = oleObject.FullObjectBin;
            Console.WriteLine("FullObjectBin data length: " + (fullObjectBinData != null ? fullObjectBinData.Length.ToString() : "null"));

            // Démontrer l'utilisation de FullObjectBin en l'enregistrant dans un fichier
            if (fullObjectBinData != null && fullObjectBinData.Length > 0)
            {
                File.WriteAllBytes("FullObjectBinData.bin", fullObjectBinData);
                Console.WriteLine("Saved FullObjectBin data to file.");
            }

            // Créer un autre classeur pour démontrer la lecture de l'objet OLE
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];

            // Ajouter l'objet OLE à partir des données FullObjectBin
            if (fullObjectBinData != null)
            {
                int newOleObjectIndex = worksheet2.OleObjects.Add(10, 10, 200, 200, fullObjectBinData, "docx");
                Console.WriteLine("Added new OLE object using FullObjectBin data.");
            }

            // Enregistrer les classeurs
            workbook.Save("OleObjectWithFullObjectBin.xlsx");
            workbook2.Save("OleObjectFromFullObjectBin.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


