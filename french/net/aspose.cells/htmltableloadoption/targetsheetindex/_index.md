---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "HtmlTableLoadOption propriété. Obtenir ou définir l'index cible de la feuille de calcul où le tableau doit être situé"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Obtenez ou définissez l'index cible de la feuille de calcul où le tableau doit être placé.

```csharp
public int TargetSheetIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Configurer les options de chargement du tableau avec TargetSheetIndex
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Ajouter des options de chargement du tableau
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // Charger le fichier HTML avec des options
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier que les tableaux ont été chargés dans les feuilles correctes
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


