---
title: "TxtLoadOptions.TextQualifier"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est '\"'.

```csharp
public char TextQualifier { get; set; }
```

### Remarques

Lors de la définition de cette propriété, [`HasTextQualifier`](../hastextqualifier/) deviendra automatiquement vrai.

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // Créer une instance de TxtLoadOptions pour CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Créer des données CSV d'exemple avec des qualificateurs de texte
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Enregistrer les données d'exemple dans un fichier temporaire
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Charger le fichier CSV avec les options spécifiées
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("TextQualifierDemo.xlsx");

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


