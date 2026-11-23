---
title: "PivotTable.DataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient et définit la source de données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Obtient et définit la source de données du tableau croisé dynamique.

```csharp
public string[] DataSource { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataSourceDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Accéder et afficher les informations de la source de données
            string[] dataSource = pivotTable.DataSource;
            Console.WriteLine("Pivot Table Data Sources:");
            foreach (string source in dataSource)
            {
                Console.WriteLine(source);
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotTableDataSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


