---
title: "Style.InvariantCustom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient la chaîne de modèle indépendante de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, null sera retourné. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera retournée."
type: docs
url: /fr/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Obtient la chaîne de modèle indépendante de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, null sera retourné. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera retournée.

```csharp
public string InvariantCustom { get; }
```

### Remarques

Pour les formats de nombre intégrés, le contenu du modèle retourné reste dépendant de la culture, par exemple, pour certains paramètres régionaux il renvoie "m/d/y" et pour d'autres il renvoie "d/m/y". La différence avec [`CultureCustom`](../culturecustom/) est (c'est aussi ce que signifie indépendant de la culture) : les spécificateurs de format et les séparateurs sont conservés comme standard, de sorte que '/' sera toujours utilisé comme séparateur de date/heure et "y" sera toujours utilisé comme partie "année" quel que soit le caractère spécial utilisé pour le paramètre régional spécifique.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Définir le format de date et la valeur
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Afficher les résultats
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


