---
title: "Classe FormatCondition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FormatCondition. Rappresenta la condizione di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatcondition/
---
## FormatCondition class

Rappresenta la condizione di formattazione condizionale.

```csharp
public class FormatCondition
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Ottieni l'istanza "AboveAverage" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle che sono al di sopra della media per tutti i valori nell'intervallo. Valida solo per type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Ottieni l'istanza "ColorScale" della formattazione condizionale. L'istanza predefinita è una "green-yellow-red" 3ColorScale. Valida solo per type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Ottieni l'istanza "DataBar" della formattazione condizionale. Il colore dell'istanza predefinita è blu. Valida solo per type = DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Ottieni l'istanza "IconSet" della formattazione condizionale. Il tipo IconSetType dell'istanza predefinita è TrafficLights31. Valida solo per type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Ottiene e imposta il tipo di operatore della formattazione condizionale. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formato deve essere valutato e renderizzato. Valori numerici più bassi hanno priorità più alta rispetto a valori numerici più alti, dove '1' è la priorità più alta. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | True, nessuna regola con priorità inferiore può essere applicata sopra questa regola, quando questa regola restituisce true. Valida solo per Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | Il valore di testo in una regola di formattazione condizionale "text contains". Valida solo per type = containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | Il periodo di tempo applicabile in una regola di formattazione condizionale "date occurrin". Valida solo per type = timePeriod. Il valore predefinito è TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Ottieni l'istanza "Top10" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle i cui valori rientrano nella fascia top 10. Valida solo per type = Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Ottiene e imposta se il tipo di formattazione condizionale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Ottiene il valore o l'espressione associati a questa condizione di formato. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Ottiene la formula della formattazione condizionale della cella. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Ottiene il valore o l'espressione associati a questa condizione di formato. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Ottiene la formula della formattazione condizionale della cella. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Imposta il valore o l'espressione associati a questa condizione di formato. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Imposta il valore o l'espressione associati a questa condizione di formato. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Imposta il valore o l'espressione associati a questa condizione di formato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // Crea un nuovo Workbook.
            Workbook workbook = new Workbook();

            // Ottieni il primo worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Aggiunge condizione.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Impostazione delle proprietà
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Dimostrazione di altre proprietà
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Salvataggio del file Excel
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


