---
title: FormatCondition
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la condizione di formattazione condizionale.
type: docs
weight: 3560
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
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Ottieni l'istanza "AboveAverage" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle che sono sopra la media per tutti i valori nell'intervallo. Valido solo per tipo = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Ottieni l'istanza "ColorScale" della formattazione condizionale. L'istanza predefinita è 3ColorScale "verde-giallo-rosso". Valido solo per tipo = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Ottieni l'istanza "DataBar" della formattazione condizionale. Il colore dell'istanza predefinita è blu. Valido solo per il tipo è DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Ottiene e imposta il valore o l'espressione associata alla formattazione condizionale. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Ottiene e imposta il valore o l'espressione associata alla formattazione condizionale. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Ottieni l'istanza "IconSet" della formattazione condizionale. IconSetType dell'istanza predefinita è TrafficLights31. Valido solo per il tipo = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Ottiene e imposta il tipo di operatore di formato condizionale. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | La priorità di questa regola di formattazione condizionale. Questo valore viene utilizzato per determinare quale formato deve essere valutato e renderizzato. I valori numerici più bassi hanno una priorità maggiore rispetto a valori numerici più alti, dove '1' è la priorità più alta. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | True, nessuna regola con priorità inferiore può essere applicata a questa regola, quando questa regola restituisce true. Vale solo per Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Ottiene o imposta lo stile degli intervalli di celle formattati condizionali. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | Il valore del testo in una regola di formattazione condizionale "il testo contiene". Valido solo per il tipo = contieneText, notContainsText, inizia con e finisce con. Il valore predefinito è null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | Il periodo di tempo applicabile in una regola di formattazione condizionale "data che si verifica...". Valido solo per tipo = timePeriod. Il valore predefinito è TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Ottieni l'istanza "Top10" della formattazione condizionale. La regola dell'istanza predefinita evidenzia le celle i cui valori rientrano nelle prime 10 parentesi. Valido solo per il tipo è Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Ottiene e imposta se il formato condizionale Type. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Ottiene il valore o l'espressione associata a questa condizione di formato. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Ottiene la formula della formattazione condizionale della cella. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Ottiene il valore o l'espressione associata a questa condizione di formato. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Ottiene la formula della formattazione condizionale della cella. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Imposta il valore o l'espressione associata a questa condizione di formato. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Imposta il valore o l'espressione associata a questa condizione di formato. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Imposta il valore o l'espressione associata a questa condizione di formato. |

### Esempi

```csharp

[C#]
//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
//Aggiunge una formattazione condizionale vuota
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
//Imposta l'intervallo di formato condizionale.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
 
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
 
//Aggiunge la condizione.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
//Aggiunge la condizione.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
//Imposta il colore di sfondo.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
//Salvataggio del file Excel
workbook.Save("output.xls");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Aggiunge una formattazione condizionale vuota
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Imposta l'intervallo di formato condizionale.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
 
'Aggiunge condizione.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Aggiunge condizione.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Imposta il colore di sfondo.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Salvataggio del file Excel
workbook.Save("output.xls")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
