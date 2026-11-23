---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient les paramètres des valeurs par défaut des propriétés liées au style pour ce classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Obtient les paramètres des valeurs par défaut des propriétés liées au style pour ce workbook.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres de style par défaut
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Définir la préférence du format numérique intégré
            styleSettings.BuiltInPreference = true;

            // Définir la culture pour le formatage des nombres
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Accéder aux cellules et appliquer le formatage
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez les valeurs et les styles
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Enregistrez le classeur
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


