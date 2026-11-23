---
title: "JsonLayoutOptions.TitleStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Obtient et définit le style du titre"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Obtient et définit le style du titre.

```csharp
public Style TitleStyle { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyTitleStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exemple de données JSON
            string jsonInput = @"
            {
                ""Name"": ""John"",
                ""Age"": 30,
                ""JoinDate"": ""2023-05-15""
            }";

            // Créer un style personnalisé pour les titres
            CellsFactory factory = new CellsFactory();
            Style titleStyle = factory.CreateStyle();
            titleStyle.HorizontalAlignment = TextAlignmentType.Center;
            titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
            titleStyle.Font.IsBold = true;

            // Configurer les options d'importation JSON
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.TitleStyle = titleStyle;
            options.ConvertNumericOrDate = true;
            options.DateFormat = "yyyy-MM-dd";

            // Importer des données JSON avec un style de titre personnalisé
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Ajuster automatiquement les colonnes pour une meilleure visibilité
            worksheet.AutoFitColumns();

            // Enregistrez le classeur
            workbook.Save("JsonWithStyledTitles.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


