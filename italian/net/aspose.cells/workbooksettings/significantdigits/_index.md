---
title: "WorkbookSettings.SignificantDigits"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta il numero di cifre significative. Il valore predefinito è SignificantDigits"
type: docs
url: /it/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Ottiene e imposta il numero di cifre significative. Il valore predefinito è [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Osservazioni

Può essere solo 15 o 17 ora. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare [`SignificantDigitsType`](../significantdigitstype/). Questa proprietà verrà rimossa 12 mesi dopo, a partire da giugno 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati numerici di esempio per dimostrare le cifre significative
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta le cifre significative a 15 (precisione massima per double)
            settings.SignificantDigits = 15;

            // Salva la cartella di lavoro per mostrare l'effetto delle cifre significative
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


