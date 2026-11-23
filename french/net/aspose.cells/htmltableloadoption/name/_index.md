---
title: "HtmlTableLoadOption.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "HtmlTableLoadOption propriété. Obtenir ou définir le nom du tableau à importer depuis le html"
type: docs
url: /fr/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Obtenir ou définir le nom du tableau à importer depuis le html

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accéder à la HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Ajouter une nouvelle HtmlTableLoadOption par indice de tableau
            int index = tableLoadOptions.Add(0);

            // Accéder à la HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Définir la propriété Name
            option.Name = "CustomerDataTable";

            // Charger un fichier HTML (remplacez par le chemin réel du fichier)
            workbook = new Workbook("input.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


