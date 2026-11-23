---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlTableLoadOptionCollection. Indique si des objets de liste sont générés à partir des tables importées. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Indique s'il faut générer des objets de liste à partir des tables importées. La valeur par défaut est false.

```csharp
public bool TableToListObject { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accédez à l'instance HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Définissez la propriété TableToListObject pour convertir les tables HTML en ListObjects
            tableLoadOptions.TableToListObject = true;

            // Ajoutez une table à convertir en ListObject par index
            tableLoadOptions.Add(0);

            // Charger un fichier HTML dans le classeur en utilisant les options de chargement
            workbook = new Workbook("input.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


