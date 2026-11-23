---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtSaveOptions. Indique si l'ajout de  pour chaque champ est toujours effectué. Si true alors toutes les valeurs seront entre guillemets. Si false alors les valeurs ne seront entre guillemets que lorsque nécessaire, par exemple lorsque les valeurs contiennent des caractères spéciaux tels que   n ou le caractère séparateur. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Indique si l'ajout de '\\"' pour chaque champ est toujours effectué. Si true, toutes les valeurs seront entre guillemets ; si false, les valeurs ne seront entre guillemets que lorsque nécessaire (par exemple, lorsque les valeurs contiennent des caractères spéciaux tels que '\\"', '\\n' ou le caractère séparateur). La valeur par défaut est false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété QuoteType. Cette propriété sera supprimée 12 mois plus tard, depuis août 2012. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // Créez TxtSaveOptions avec AlwaysQuoted défini sur true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Enregistrez avec des guillemets autour de toutes les valeurs
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // Modifiez en false et enregistrez à nouveau
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### Voir aussi

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


