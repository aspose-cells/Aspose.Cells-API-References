---
title: "Cells.ImportDataRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe un DataRow dans le fichier Excel"
type: docs
url: /fr/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Importe une DataRow dans le fichier Excel.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataRow | DataRow | Objet DataRow. |
| ligne | Int32 | Index de ligne. |
| firstColumn | Int32 | Indice de première colonne. |

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créez un DataTable d'exemple
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Ajoutez des données d'exemple
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Importer la première ligne du DataTable vers la feuille de calcul en commençant à la ligne 0, colonne 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Enregistrez le classeur
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


