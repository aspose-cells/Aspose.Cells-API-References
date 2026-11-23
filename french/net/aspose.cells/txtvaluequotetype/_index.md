---
title: "Enum TxtValueQuoteType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.TxtValueQuoteType enum. Spécifie le type d'utilisation des guillemets pour les valeurs dans les fichiers au format texte"
type: docs
url: /fr/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Spécifie le type d'utilisation des guillemets pour les valeurs dans les fichiers au format texte.

```csharp
public enum TxtValueQuoteType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Normal | `0` | Toutes les valeurs contenant des caractères spéciaux tels que les guillemets ou le caractère de séparation seront entre guillemets. Même comportement que celui de MS Excel lors de l'exportation d'un fichier texte. |
| Always | `1` | Toutes les valeurs seront toujours entre guillemets. |
| Minimum | `2` | Entourez les valeurs de guillemets uniquement lorsque c'est nécessaire. Par exemple, si une valeur contient un guillemet mais que le guillemet n'est pas au début de cette valeur, cette valeur ne sera pas entre guillemets. |
| Never | `3` | Aucune valeur ne sera entre guillemets. Le fichier texte exporté avec ce type peut ne pas être relu correctement parce que les guillemets nécessaires sont absents. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // Créer TxtSaveOptions et définir le QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Enregistrer le classeur en tant que fichier texte avec le type de guillemet spécifié
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


