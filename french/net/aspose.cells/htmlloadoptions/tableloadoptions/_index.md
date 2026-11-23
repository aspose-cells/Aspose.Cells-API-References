---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Obtient l'instance HtmlTableLoadOptionCollection"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

Obtenir l'instance HtmlTableLoadOptionCollection

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Ajouter des options de chargement de tableau par index
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // Ajouter des options de chargement de tableau par ID
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Chargez le fichier HTML avec les options
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Enregistrer la sortie
            workbook.Save("output.xlsx");
            
            // Effacer et ajouter de nouvelles options de chargement de tableau
            loadOptions.TableLoadOptions.Clear();
            
            // Ajouter des options de chargement de tableau avec mappage d'index de feuille
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // Ajouter des options de chargement de tableau avec ID et mappage de feuille
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Charger et enregistrer à nouveau avec de nouvelles options
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


