---
title: "QueryTable.AdjustColumnWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété QueryTable. Retourne ou définit AdjustColumnWidth de l’objet"
type: docs
url: /fr/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Renvoie ou définit AdjustColumnWidth de l'objet.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d’exemple avec des largeurs de colonne variables
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Définir manuellement les largeurs de colonne
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Créer une table de requête (simulée car la création réelle nécessite une source de données externe)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Afficher la valeur actuelle de AdjustColumnWidth
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // Définir AdjustColumnWidth sur true et démontrer l’effet
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Simuler le rafraîchissement de la table de requête (ajusterait normalement les largeurs de colonne)
            // Dans un scénario réel, cela se produirait lorsque la table de requête rafraîchit ses données
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // Définir AdjustColumnWidth sur false et démontrer l’effet
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Simuler un nouveau rafraîchissement (conserverait maintenant les largeurs de colonne d’origine)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Enregistrez le classeur
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


