---
title: "Cells.ImportDataView"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe un DataView dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Importe une DataView dans une feuille de calcul.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataView | DataView | L’objet DataView à importer. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |

### Valeur de retour

Nombre total de lignes importées

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un DataTable d’exemple
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Ajoutez des données d'exemple
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // Créer DataView à partir de DataTable
            DataView dataView = new DataView(table);

            // Importer DataView dans la feuille de calcul en commençant à la ligne 0, colonne 0
            cells.ImportDataView(dataView, 0, 0);

            // Enregistrez le classeur
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


