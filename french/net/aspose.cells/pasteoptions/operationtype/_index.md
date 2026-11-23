---
title: "PasteOptions.OperationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PasteOptions. Obtient et définit le type d'opération lors du collage de la plage"
type: docs
url: /fr/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Obtient et définit le type d'opération lors du collage de la plage.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Créer le classeur source avec des données d'exemple
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Créer le classeur de destination
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Créer des plages pour copier/coller
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // Créer des options de collage avec une démonstration d'OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Effectuer l'opération de copier/coller
            rangeDestination.Copy(rangeOrigin, options);
            
            // Vérifier le résultat
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Enregistrer le résultat
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


