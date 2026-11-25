---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene le impostazioni per i valori predefiniti delle proprietà correlate allo stile per questa cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Ottiene le impostazioni per i valori predefiniti delle proprietà relative allo stile per questa workbook.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni di stile predefinite
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Imposta la preferenza del formato numerico incorporato
            styleSettings.BuiltInPreference = true;

            // Imposta la cultura per la formattazione dei numeri
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Accedi alle celle e applica la formattazione
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta valori e stili
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Salva la cartella di lavoro
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


