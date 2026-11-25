---
title: "Classe PivotGlobalizationSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Settings.PivotGlobalizationSettings classe. Rappresenta le impostazioni di globalizzazione per le tabelle pivot"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/
---
## PivotGlobalizationSettings class

Rappresenta le impostazioni di globalizzazione per le tabelle pivot.

```csharp
public class PivotGlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotGlobalizationSettings](pivotglobalizationsettings/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [GetFormatOfDayGroup](../../aspose.cells.settings/pivotglobalizationsettings/getformatofdaygroup/)() | Ottiene il formato numerico del gruppo giorno pivot. Utilizzato solo quando si raggruppa il campo pivot per giorni. Il valore predefinito è "d-MMM"; |
| virtual [GetNameOfDataField](../../aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/)(ConsolidationFunction, string) | Ottiene il nome visualizzato del campo pivot dei dati. Il formato predefinito è "Sum Of Field". |
| virtual [GetShortTextOf12Months](../../aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/)() | Ottiene tutte le stringhe brevi formattate dei 12 mesi. |
| virtual [GetTextOf24Hours](../../aspose.cells.settings/pivotglobalizationsettings/gettextof24hours/)() | Ottiene tutte le stringhe formattate localmente delle 24 ore. Il valore predefinito è 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| virtual [GetTextOf4Quarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quarters/)() | Ottiene il testo locale di 4 trimestri. |
| virtual [GetTextOf4Quaters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/)() | (**Obsolete.**) Ottiene il testo locale di 4 trimestri. |
| virtual [GetTextOfAll](../../aspose.cells.settings/pivotglobalizationsettings/gettextofall/)() | Restituisce il testo dell'etichetta "(All)" nella PivotTable. |
| virtual [GetTextOfAllPeriods](../../aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/)() | Ottiene il testo localizzato di "All Periods". |
| virtual [GetTextOfColumnLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/)() | Restituisce il testo dell'etichetta "Column Labels" nella PivotTable. |
| virtual [GetTextOfDataFieldHeader](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/)() | Restituisce il testo dell'intestazione del campo dell'area valori nella PivotTable. |
| virtual [GetTextOfDays](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdays/)() | Ottiene il testo locale di "Days". |
| virtual [GetTextOfEmptyData](../../aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/)() | Restituisce il testo dell'etichetta "(blank)" nella PivotTable. |
| virtual [GetTextOfGrandTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/)() | Restituisce il testo dell'etichetta "Grand Total" nella PivotTable. |
| virtual [GetTextOfHours](../../aspose.cells.settings/pivotglobalizationsettings/gettextofhours/)() | Ottiene il testo locale di "Hours". |
| virtual [GetTextOfMinutes](../../aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/)() | Ottiene il testo locale di "Minutes". |
| virtual [GetTextOfMonths](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/)() | Ottiene il testo locale di "Months". |
| virtual [GetTextOfMultipleItems](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/)() | Restituisce il testo dell'etichetta "(Multiple Items)" nella PivotTable. |
| virtual [GetTextOfOr](../../aspose.cells.settings/pivotglobalizationsettings/gettextofor/)() | Ottiene tutte le stringhe formattate localmente di "or". |
| virtual [GetTextOfProtectedName](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/)(string) | Restituisce il testo per il nome protetto specificato. |
| virtual [GetTextOfProtection](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/)() | (**Obsolete.**) Ottiene il nome della protezione nella Tabella Pivot. |
| virtual [GetTextOfQuarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/)() | Ottieni il testo locale di "Quarters". |
| virtual [GetTextOfRange](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrange/)() | Ottiene il testo locale di "Range" |
| virtual [GetTextOfRowLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/)() | Restituisce il testo dell'etichetta "Row Labels" nella PivotTable. |
| virtual [GetTextOfSeconds](../../aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/)() | Ottiene il testo locale di "Seconds" |
| virtual [GetTextOfSubTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/)(PivotFieldSubtotalType) | Restituisce il testo del tipo [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) nella PivotTable. |
| virtual [GetTextOfTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/)() | Restituisce il testo dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati. |
| virtual [GetTextOfYears](../../aspose.cells.settings/pivotglobalizationsettings/gettextofyears/)() | Ottiene il testo locale di "Years". |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGlobalizationSettingsDemo
    {
        public static void PivotGlobalizationSettingsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["B5"].PutValue(250);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea un'istanza di PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Dimostrare l'uso di vari metodi
            Console.WriteLine("Text of Total: " + globalizationSettings.GetTextOfTotal());
            Console.WriteLine("Text of Grand Total: " + globalizationSettings.GetTextOfGrandTotal());
            Console.WriteLine("Text of Multiple Items: " + globalizationSettings.GetTextOfMultipleItems());
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());
            Console.WriteLine("Text of Protection: " + globalizationSettings.GetTextOfProtection());
            Console.WriteLine("Text of Column Labels: " + globalizationSettings.GetTextOfColumnLabels());
            Console.WriteLine("Text of Row Labels: " + globalizationSettings.GetTextOfRowLabels());
            Console.WriteLine("Text of Empty Data: " + globalizationSettings.GetTextOfEmptyData());
            Console.WriteLine("Text of Data Field Header: " + globalizationSettings.GetTextOfDataFieldHeader());
            Console.WriteLine("Text of Years: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Text of Quarters: " + globalizationSettings.GetTextOfQuarters());
            Console.WriteLine("Text of Months: " + globalizationSettings.GetTextOfMonths());
            Console.WriteLine("Text of Days: " + globalizationSettings.GetTextOfDays());
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

            // Esempio del metodo GetTextOfProtectedName
            string protectedName = "ProtectedNameExample";
            Console.WriteLine("Text of Protected Name: " + globalizationSettings.GetTextOfProtectedName(protectedName));

            // Esempio del metodo GetTextOfSubTotal
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine("Text of SubTotal (Sum): " + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // Salva la cartella di lavoro
            workbook.Save("PivotGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Settings](../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../)


