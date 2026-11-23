---
title: "Workbook.Combine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Combine un autre objet Workbook"
type: docs
url: /fr/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Combine un autre objet Workbook.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| secondWorkbook | Classeur | Un autre objet Workbook. |

### Remarques

Fusionner Excel, ODS, CSV et d’autres fichiers en un seul fichier.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Créer le classeur source
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Combiner les classeurs
            destWorkbook.Combine(sourceWorkbook);

            // Enregistrer le classeur combiné
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


