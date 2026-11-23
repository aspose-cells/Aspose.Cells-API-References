---
title: "Énumération TxtLoadStyleStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.TxtLoadStyleStrategy. Spécifie comment appliquer le style aux valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure"
type: docs
url: /fr/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Spécifie comment appliquer le style aux valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure.

```csharp
public enum TxtLoadStyleStrategy
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Ne définit pas de style pour la valeur analysée. |
| BuiltIn | `1` | Définit le style comme nombre/date‑heure intégré lorsque la valeur analysée est une valeur numérique/date‑heure simple. |
| ExactFormat | `2` | Définit le format personnalisé exact pour la valeur analysée afin que la valeur formatée soit identique à l'entrée originale. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir un contenu CSV d'exemple
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // Enregistrer le contenu CSV dans un fichier temporaire
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // Créer TxtLoadOptions et définir le LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // Charger le fichier CSV dans le classeur
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Nettoyer le fichier CSV temporaire
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


