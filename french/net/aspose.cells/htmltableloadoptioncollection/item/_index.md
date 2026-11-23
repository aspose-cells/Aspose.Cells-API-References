---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlTableLoadOptionCollection. Obtient l’élément HtmlTableLoadOption à l’index spécifié"
type: docs
url: /fr/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Obtient l’élément [`HtmlTableLoadOption`](../../htmltableloadoption/) à l’index spécifié.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ajouter une nouvelle HtmlTableLoadOption par indice de tableau
            int index1 = tableLoadOptions.Add(0);

            // Accéder au HtmlTableLoadOption en utilisant la propriété Item
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Configurer l’option de chargement du tableau
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Charger le fichier HTML avec les options configurées
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


