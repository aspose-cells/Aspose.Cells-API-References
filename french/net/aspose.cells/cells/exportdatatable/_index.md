---
title: "Cells.ExportDataTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Exporte les données de la collection Cells vers un objet DataTable"
type: docs
url: /fr/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Exporte les données de la collection [`Cells`](../) vers un objet DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
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

Si vous utilisez cette méthode pour exporter un bloc de données, assurez-vous que les données d'une colonne soient du même type. Sinon, utilisez la méthode [`ExportDataTableAsString`](../exportdatatableasstring/) à la place.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // Exporter les données vers DataTable (en commençant à la ligne 0, colonne 0, avec 5 lignes et 3 colonnes)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // Afficher les données exportées
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
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

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Exporte les données de la collection [`Cells`](../) vers un objet DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
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

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
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

            // Exporter les données vers DataTable (la première ligne contient les en-têtes)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // Afficher les données exportées
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
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

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Exporte les données de la collection [`Cells`](../) vers un objet DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| totalRows | Int32 | Nombre de lignes à importer. |
| totalColumns | Int32 | Nombre de colonnes à importer. |
| options | ExportTableOptions | Toutes les options d'exportation de tableau |

### Valeur de retour

Objet DataTable exporté.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Définir la valeur et le format pour la cellule A1
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // Créez des options d'exportation
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // Exporter avec la stratégie de format CellStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // Exporter avec la stratégie de format None
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // Exporter avec la stratégie de format DisplayStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


