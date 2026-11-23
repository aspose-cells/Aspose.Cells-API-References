---
title: "Énumération AutoFitWrappedTextType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.AutoFitWrappedTextType enum. Représente le type de texte enveloppé ajusté automatiquement"
type: docs
url: /fr/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Représente le type d'ajustement automatique du texte renvoyé à la ligne.

```csharp
public enum AutoFitWrappedTextType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Fonctionne comme MS Excel. |
| Paragraph | `1` | Ajuster automatiquement la largeur avec le paragraphe le plus long. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // Créer une plage A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Fusionner les cellules
            range.Merge();

            // Créer une plage A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Fusionner les cellules
            range2.Merge();

            // Créer AutoFitterOptions et définir AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Ajuster automatiquement les lignes avec les options spécifiées
            worksheet.AutoFitRows(options);

            // Enregistrez le classeur
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


