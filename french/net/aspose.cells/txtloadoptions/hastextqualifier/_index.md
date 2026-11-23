---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Indique s'il existe un qualificateur de texte pour la valeur de cellule. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Indique s'il existe un qualificateur de texte pour la valeur de cellule. La valeur par défaut est true.

```csharp
public bool HasTextQualifier { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Créez du contenu CSV avec des qualificateurs de texte
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // Enregistrez le contenu CSV dans un fichier temporaire
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // Créez TxtLoadOptions avec HasTextQualifier défini sur true
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Chargez le fichier CSV avec des qualificateurs de texte
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Enregistrez le classeur pour démontrer le chargement réussi
            workbook.Save("Output.xlsx");

            // Supprimer le fichier temporaire
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


