---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Si true, convertit la chaîne en formule lorsque la valeur de la chaîne commence par le caractère ; la valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

Si true, convertit la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlLoadOptions.HasFormula. Cette propriété sera supprimée 12 mois après mars 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // Créer une instance de HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Définissez la propriété ConvertFormulasData sur true
            options.ConvertFormulasData = true;

            // Charger un fichier HTML dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("input.html", options);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher certaines valeurs de cellules pour démontrer la conversion de formules
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

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


