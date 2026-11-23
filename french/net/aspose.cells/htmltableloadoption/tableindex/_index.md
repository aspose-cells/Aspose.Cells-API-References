---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "HtmlTableLoadOption propriété. Obtenir ou définir l'index du tableau à importer depuis le html"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Obtenez ou définissez l'index du tableau à importer depuis html.

```csharp
public int TableIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Configurer l'option de chargement du tableau avec TableIndex = 0 (premier tableau)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Ajouter l'option de chargement du tableau
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Charger le fichier HTML (remplacez par le chemin réel)
            workbook = new Workbook("input.html", loadOptions);

            // Enregistrer en tant que fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


