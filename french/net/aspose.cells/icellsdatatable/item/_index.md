---
title: "ICellsDataTable.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ICellsDataTable. Obtient les données stockées dans la colonne spécifiée par l'index"
type: docs
url: /fr/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Obtient les données stockées dans la colonne spécifiée par l'index.

```csharp
public object this[int columnIndex] { get; }
```

| Paramètre | Description |
| --- | --- |
| columnIndex | L'index de la colonne basé sur zéro. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Créer un ICellsDataTable personnalisé avec des données d'exemple
            ICellsDataTable dataTable = new SampleDataTable();

            // Réinitialiser la position du curseur
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Accéder aux valeurs par index de colonne
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Accéder aux valeurs par nom de colonne
                Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
            }
        }
    }

    internal class SampleDataTable : ICellsDataTable
    {
        private readonly string[] columns = { "Product", "Price", "Stock" };
        private readonly object[][] data = 
        {
            new object[] { "Laptop", 999.99, 15 },
            new object[] { "Phone", 699.99, 25 },
            new object[] { "Tablet", 299.99, 50 }
        };
        private int currentRow = -1;

        public string[] Columns => columns;
        public int Count => data.Length;

        public object this[int columnIndex] => data[currentRow][columnIndex];
        public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];

        public void BeforeFirst() => currentRow = -1;
        public bool Next() => ++currentRow < data.Length;
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Obtient les données stockées dans la colonne spécifiée par le nom de colonne.

```csharp
public object this[string columnName] { get; }
```

| Paramètre | Description |
| --- | --- |
| columnName | Le nom de la colonne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les cellules avec des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Exporter la plage de données vers ICellsDataTable avec un cast explicite
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // Se déplacer avant le premier enregistrement
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Accéder à la propriété Item en utilisant les noms de colonnes (indexeur)
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Enregistrez le classeur
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


