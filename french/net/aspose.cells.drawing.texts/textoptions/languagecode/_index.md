---
title: "TextOptions.LanguageCode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Obtient et définit la langue de l'interface utilisateur"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Obtient et définit la langue de l'interface utilisateur.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme et définissez son texte
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Définissez le code de langue pour les options de texte de la forme
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Vérifiez et affichez le code de langue
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Enregistrez le classeur
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


