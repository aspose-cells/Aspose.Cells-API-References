---
title: "Style.CultureCustom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient et définit la chaîne de modèle dépendante de la culture pour le format de nombre. Si aucun format de nombre n’a été défini pour cet objet, null sera renvoyé. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée."
type: docs
url: /fr/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Obtient et définit la chaîne de modèle dépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera retourné. Si le format numérique est intégré, la chaîne de modèle correspondant au numéro intégré sera retournée.

```csharp
public string CultureCustom { get; set; }
```

### Remarques

Pour les formats de nombre intégrés, à la fois le contenu du modèle (par exemple, un format de date intégré est "m/d/y" pour certains paramètres régionaux, mais pour d’autres il devient "d/m/y") et le spécificateur de format (par exemple, certains paramètres régionaux utilisent un caractère différent de 'y' pour représenter la partie année du format de date) sont dépendants de la culture ; pour un format personnalisé spécifié par l’utilisateur, seuls les spécificateurs de format sont modifiés selon la culture, les autres parties du modèle de format ne seront pas modifiées.

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Créez un classeur et définissez la culture hongroise
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // Obtenez la première cellule et son style
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Définissez un format personnalisé et démontrez la conversion CultureCustom
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Appliquez le style et démontrez le formatage sensible à la culture
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Démontrez une formule avec le formatage culturel
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


