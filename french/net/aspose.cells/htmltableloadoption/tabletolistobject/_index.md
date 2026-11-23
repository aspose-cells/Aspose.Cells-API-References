---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "HtmlTableLoadOption propriété. Indique si des objets de liste sont générés à partir du tableau importé. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Indique si des objets de liste doivent être générés à partir du tableau importé. La valeur par défaut est false.

```csharp
public bool TableToListObject { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer des options de chargement HTML avec TableToListObject activé
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Charger le HTML avec les options spécifiées
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


