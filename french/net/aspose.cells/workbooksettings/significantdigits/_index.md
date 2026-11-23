---
title: "WorkbookSettings.SignificantDigits"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est SignificantDigits"
type: docs
url: /fr/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Remarques

Il ne peut être que 15 ou 17 maintenant. NOTE : Ce membre est désormais obsolète. À la place, veuillez utiliser [`SignificantDigitsType`](../significantdigitstype/). Cette propriété sera supprimée 12 mois plus tard, à compter de juin 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données numériques d'exemple pour démontrer les chiffres significatifs
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir les chiffres significatifs à 15 (précision maximale pour double)
            settings.SignificantDigits = 15;

            // Enregistrer le classeur pour montrer l'effet des chiffres significatifs
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


