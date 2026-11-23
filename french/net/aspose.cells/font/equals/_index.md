---
title: "Font.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Font. Vérifie si deux polices sont égales"
type: docs
url: /fr/net/aspose.cells/font/equals/
---
## Font.Equals method

Vérifie si deux polices sont égales.

```csharp
public bool Equals(Font font)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| police | Police | Objet police comparé. |

### Valeur de retour

Vrai si égal à l'objet police comparé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux objets police à comparer
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Appeler la méthode Equals pour comparer les polices
                bool areEqual = font1.Equals(font2);

                // Afficher le résultat
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Modifier une police pour les rendre différentes
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


