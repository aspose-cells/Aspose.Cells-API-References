---
title: "HtmlTableLoadOption.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "HtmlTableLoadOption property. Obtenir ou définir l'identifiant du tableau à importer depuis le HTML"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Obtenez ou définissez l'id du tableau à importer depuis html

```csharp
public string Id { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Configurer les options de chargement du tableau
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Ajouter des options de chargement du tableau
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Charger le fichier HTML avec les options spécifiées
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


