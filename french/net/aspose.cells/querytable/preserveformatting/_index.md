---
title: "QueryTable.PreserveFormatting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété QueryTable. Retourne ou définit le PreserveFormatting de l'objet"
type: docs
url: /fr/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Renvoie ou définit PreserveFormatting de l'objet.

```csharp
public bool PreserveFormatting { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple et le formatage
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Appliquer le formatage à la plage de données
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Appliquer le style à chaque cellule de la plage
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Créer une table de requête (simulée car la création réelle nécessite une source de données externe)
            // Dans une utilisation réelle, vous créeriez cela à partir d'une connexion externe
            QueryTable queryTable = worksheet.QueryTables[0];

            // Afficher la valeur actuelle de PreserveFormatting
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // Définir PreserveFormatting sur false (ne préserve pas le formatage existant lors du rafraîchissement)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simuler le rafraîchissement du tableau de requête (effacerait normalement le formatage lorsque PreserveFormatting est false)
            // Dans un scénario réel, cela se produirait lorsque la table de requête rafraîchit ses données
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // Redéfinir PreserveFormatting sur true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simuler un nouveau rafraîchissement (préserverait maintenant le formatage)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Enregistrez le classeur
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


