---
title: "Cells.ExportDataTableAsString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Exporte les données de la collection Cells vers un objet DataTable"
type: docs
url: /fr/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Exporte les données de la collection [`Cells`](../) vers un objet DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| totalRows | Int32 | Nombre de lignes à importer. |
| totalColumns | Int32 | Nombre de colonnes à importer. |

### Valeur de retour

Objet DataTable exporté.

### Remarques

Toutes les données de la collection [`Cells`](../) sont converties en chaînes.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple aux cellules
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Exporter les données vers DataTable sous forme de chaînes
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Afficher les données exportées
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Exporte les données de la collection [`Cells`](../) vers un objet DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| totalRows | Int32 | Nombre de lignes à importer. |
| totalColumns | Int32 | Nombre de colonnes à importer. |
| exportColumnName | Boolean | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. |

### Valeur de retour

Objet DataTable exporté.

### Remarques

Toutes les données de la collection [`Cells`](../) sont converties en chaînes.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Exporter les données vers DataTable
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Afficher les données exportées
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


