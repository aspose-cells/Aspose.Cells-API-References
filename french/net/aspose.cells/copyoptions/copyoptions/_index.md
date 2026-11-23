---
title: "CopyOptions.CopyOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur CopyOptions. Constructeur CopyOptions"
type: docs
url: /fr/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

Constructeur CopyOptions.

```csharp
public CopyOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et obtenir la première feuille
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Ajouter des données d'exemple à la feuille source
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // Créer CopyOptions en utilisant le constructeur
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Copier les lignes avec les options
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Enregistrez le classeur
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


