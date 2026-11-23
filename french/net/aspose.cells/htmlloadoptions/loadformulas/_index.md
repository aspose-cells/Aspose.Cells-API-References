---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Indique s'il faut importer les formules si le fichier HTML original contient des formules"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Indique s'il faut importer les formules si le fichier html original en contient.

```csharp
public bool LoadFormulas { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // Créer une instance de HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Définissez LoadFormulas sur true pour charger les formules depuis le HTML
            loadOptions.LoadFormulas = true;

            // Charger un fichier HTML contenant des formules dans un classeur
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher la formule de la cellule A1 (si présente dans le HTML)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


