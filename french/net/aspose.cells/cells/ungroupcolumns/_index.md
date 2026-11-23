---
title: "Cells.UngroupColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Dissocie les colonnes"
type: docs
url: /fr/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Dégroupe les colonnes.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de colonne à dissocier. |
| lastIndex | Int32 | Le dernier indice de colonne à dissocier. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Regroupez d'abord les colonnes pour démontrer la dissociation
            worksheet.Cells.GroupColumns(0, 2);

            // Dissociez les colonnes (0 à 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


