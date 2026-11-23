---
title: "Classe JsonLayoutOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Utility.JsonLayoutOptions. Représente les options du type de mise en page json"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Représente les options du type de mise en page JSON.

```csharp
public class JsonLayoutOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Constructeur de chargement des options de mise en page JSON. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Traite le tableau comme une table. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Indique si la conversion de la chaîne en json en valeur numérique ou date est effectuée. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Obtient et définit le format de la valeur de date. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Indique s'il faut ignorer le titre si le tableau est une propriété d'un objet. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Indique s'il faut ignorer les valeurs nulles. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Indique s'il faut ignorer le titre si l'objet est une propriété d'un autre objet. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ignore les titres des attributs |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Indique s'il faut conserver le schéma de ce JSON. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Obtient et définit le format de la valeur numérique. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Obtient et définit le style du titre. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassJsonLayoutOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez JsonLayoutOptions et définissez les propriétés
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Exemple de données JSON
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // Importez les données JSON dans la feuille de calcul
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Enregistrez le classeur
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


