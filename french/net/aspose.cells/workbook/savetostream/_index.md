---
title: "Workbook.SaveToStream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Enregistre le fichier Excel dans un objet MemoryStream en tant que fichier Excel972003 xls et le renvoie"
type: docs
url: /fr/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Enregistre le fichier Excel dans un objet MemoryStream en tant que fichier xls Excel97-2003 et le renvoie.

```csharp
public MemoryStream SaveToStream()
```

### Valeur de retour

Objet MemoryStream contenant un fichier Excel xls.

### Remarques

Cette méthode fournit la même fonction que la méthode Save et enregistre uniquement le classeur au format Excel97-2003 xls. Elle est principalement destinée aux appels depuis des clients COM.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook start = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter des données d'exemple
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Enregistrer le classeur dans un MemoryStream
            MemoryStream stream = start.SaveToStream();

            // Créer un nouveau classeur à partir du flux
            Workbook workbook = new Workbook(stream);

            // Modifier le nouveau classeur
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


