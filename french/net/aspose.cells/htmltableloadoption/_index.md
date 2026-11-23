---
title: "Classe HtmlTableLoadOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.HtmlTableLoadOption. Représente l'option lors de l'importation d'un tableau depuis HTML"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

Représente l'option lors de l'importation d'un tableau depuis HTML.

```csharp
public class HtmlTableLoadOption
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Obtenez ou définissez l'id du tableau à importer depuis html |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) Obtenez ou définissez le nom du tableau à importer depuis html |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Obtenez ou définissez l'index original de la feuille de calcul dans le html. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Obtenez ou définissez l'index du tableau à importer depuis html. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Indique si des objets de liste doivent être générés à partir du tableau importé. La valeur par défaut est false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Obtenez ou définissez l'index cible de la feuille de calcul où le tableau doit être placé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une instance de HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Créer une instance de HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Ajouter le HtmlTableLoadOption aux HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Charger le fichier HTML dans le classeur avec les options de chargement spécifiées
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


