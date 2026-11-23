---
title: "Cells.ImportData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe des données d'un objet IDataReader"
type: docs
url: /fr/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

Importe des données d'un objet IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| lecteur | IDataReader | L'objet IDataReader qui contient des données. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |

### Valeur de retour

Nombre total de lignes importées.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataWithIDataReaderInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une table de données d'exemple
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // Créer un IDataReader à partir d'une DataTable
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // Appeler la méthode ImportData en commençant à la cellule A1 (ligne 0, colonne 0)
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Ajuster automatiquement les colonnes pour une meilleure visibilité
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

Importe des données d'un objet IDataReader.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| lecteur | IDataReader | L'objet IDataReader qui contient des données. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |
| options | ImportTableOptions | Les options d'importation de la table. |

### Valeur de retour

Nombre total de lignes importées.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithIDataReaderInt32Int32ImportTabDemo
    {
        public static void Run()
        {
            // Créez un DataTable d'exemple
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // Ajoutez des données d'exemple
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // Créer un DataTableReader
            DataTableReader reader = dt.CreateDataReader();

            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les options d'importation
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // Importer des données en commençant à la ligne 5, colonne 0
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // Enregistrez le classeur
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Importe des données d'une table de données personnalisée.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| table | ICellsDataTable | La table de données personnalisée. |
| firstRow | Int32 | Indice de la première ligne. |
| firstColumn | Int32 | Indice de première colonne. |
| options | ImportTableOptions | Les options d'importation |

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithICellsDataTableInt32Int32ImporDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            ArrayList dataLists = new ArrayList();
            dataLists.Add(new object[] { "Name", "Age", "Gender" });
            dataLists.Add(new object[] { "Alice", 30, "Female" });
            dataLists.Add(new object[] { "Bob", 25, "Male" });
            dataLists.Add(new object[] { "Charlie", 35, "Male" });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            
            Console.WriteLine("Data imported to first worksheet:");
            Console.WriteLine(wb.Worksheets[0].Cells["A2"].StringValue);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Importe des données d'une table de données personnalisée.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| table | DataTable | L'objet DataTable à importer. |
| firstRow | Int32 | Indice de la première ligne. |
| firstColumn | Int32 | Indice de première colonne. |
| options | ImportTableOptions | Les options d'importation |

### Valeur de retour

Nombre total de lignes importées.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataTableInt32Int32ImportTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Créer un DataTable d’exemple
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // Ajoutez des données d'exemple
            DataRow row = dataTable.NewRow();
            row[0] = 1;
            row[1] = "Aniseed Syrup";
            row[2] = 15;
            dataTable.Rows.Add(row);

            row = dataTable.NewRow();
            row[0] = 2;
            row[1] = "Boston Crab Meat";
            row[2] = 123;
            dataTable.Rows.Add(row);

            // Définir les options d'importation
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // Importer les données à partir de la ligne 5, colonne 5
            cells.ImportData(dataTable, 5, 5, importOptions);

            // Enregistrez le classeur
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Importe des données d'une vue de données.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataView | DataView | L’objet DataView à importer. |
| firstRow | Int32 | Indice de la première ligne. |
| firstColumn | Int32 | Indice de première colonne. |
| options | ImportTableOptions | Les options d'importation |

### Valeur de retour

Nombre total de lignes importées.

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataViewInt32Int32ImportTableODemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Créer une table de données d'exemple
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // Ajoutez des données d'exemple
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // Créer ImportTableOptions
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // Importer les données de DataView vers les cellules à partir de la ligne 0, colonne 0
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // Enregistrez le classeur
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


