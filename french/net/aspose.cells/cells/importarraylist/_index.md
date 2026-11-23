---
title: "Cells.ImportArrayList"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe une ArrayList de données dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Importe une ArrayList de données dans une feuille de calcul.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| arrayList | ArrayList | ArrayList de données. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| isVertical | Boolean | Spécifie d'importer les données verticalement ou horizontalement. |

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportArrayListWithArrayListInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ArrayList data = new ArrayList();
            data.Add("Name");
            data.Add("Age");
            data.Add("City");
            
            cells.ImportArrayList(data, 0, 0, false);
            
            data.Clear();
            data.Add("John");
            data.Add(30);
            data.Add("New York");
            
            cells.ImportArrayList(data, 1, 0, false);
            
            workbook.Save("ImportArrayListDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


