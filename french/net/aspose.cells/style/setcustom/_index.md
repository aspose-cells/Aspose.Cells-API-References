---
title: "Style.SetCustom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Définit la chaîne de format numérique personnalisé d'une cellule"
type: docs
url: /fr/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Définit la chaîne de format numérique personnalisée d'une cellule.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| personnalisé | String | Chaîne de format numérique personnalisé, doit être un motif InvariantCulture. |
| builtinPreference | Boolean | Si la chaîne de format numérique personnalisé fournie correspond à l'un des formats numériques intégrés correspondant aux paramètres régionaux actuels, indique s'il faut définir le format numérique comme intégré plutôt que personnalisé. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


