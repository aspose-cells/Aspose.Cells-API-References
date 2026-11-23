---
title: "StyleFlag.QuotePrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre Hide formula sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

Le paramètre de masquage de formule sera appliqué.

```csharp
public bool QuotePrefix { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la cellule A1 et définissez une valeur qui ressemble à un nombre mais qui doit être traitée comme du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // Créez un style et définissez QuotePrefix sur true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // Créez un indicateur de style et activez le drapeau QuotePrefix
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // Appliquez le style à la cellule en utilisant SetStyle au lieu de ApplyStyle
            cell.SetStyle(style, flag);

            // Affichez la valeur actuelle de QuotePrefix
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // Enregistrez le classeur pour voir l'effet (la valeur sera traitée comme du texte dans Excel)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // Maintenant, changeons QuotePrefix à false et voyons la différence
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // Enregistrez à nouveau avec un nom différent pour comparer
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


