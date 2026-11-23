---
title: "WorkbookDesigner.SortDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookDesigner. Indique si la source de données est triée"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Indique si la source de données est triée.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. Cette propriété sera supprimée 12 mois plus tard à compter d’octobre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer. La source de données Json sera triée si le marqueur intelligent contient des paramètres ascendants et descendants.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // Créer un DataTable d'exemple avec des données non triées
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Ajouter des données d'exemple dans un ordre non trié
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Créer un classeur avec des marqueurs intelligents
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configurer les smart markers dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // Créer une instance de WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Afficher la valeur initiale de SortDataSource
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Définir la source de données sans tri
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Enregistrer le résultat non trié
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Créer un nouveau classeur pour la démonstration triée
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Créer un nouveau concepteur avec le tri activé
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Enregistrer le résultat trié
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


