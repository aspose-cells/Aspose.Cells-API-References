---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta il tipo di cifre significative per la visualizzazione dei valori numerici in questa cartella di lavoro. Il valore predefinito è SignificantDigitsType"
type: docs
url: /it/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

Ottiene e imposta il tipo di cifre significative per la visualizzazione dei valori numerici in questa cartella di lavoro. Il valore predefinito è [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Visualizza il valore corrente di SignificantDigitsType
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // Dimostra l'impostazione di valori diversi di SignificantDigitsType
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // Aggiungi alcuni dati numerici per dimostrare l'effetto
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // Salva la cartella di lavoro
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### Vedi anche

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


