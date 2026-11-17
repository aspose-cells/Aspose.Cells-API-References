---
title: "FormatCondition Class"
linktitle: "FormatCondition"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "FormatCondition class. Incapsula l'oggetto che rappresenta formatcondition in Go."
type: docs
weight: 200
url: /it/go-cpp/formatcondition/
---

## FormatCondition class

Rappresenta la condizione di formattazione condizionale.

```go

type FormatCondition struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Ottiene il valore o l'espressione associati a questa condizione di formattazione. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Ottiene il valore o l'espressione associati a questa condizione di formattazione. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Ottiene il valore o l'espressione della formattazione condizionale della cella. |
| [SetFormulas](./setformulas/) | Imposta il valore o l'espressione associati a questa condizione di formattazione. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Imposta il valore o l'espressione associati a questa condizione di formattazione. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Imposta il valore o l'espressione associati a questa condizione di formattazione. |
| [GetFormula1](./getformula1/) | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale. |
| [SetFormula1_String](./setformula1_string/) | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | Ottiene la formula della formattazione condizionale della cella. |
| [GetFormula2](./getformula2/) | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale. |
| [SetFormula2_String](./setformula2_string/) | Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | Ottiene la formula della formattazione condizionale della cella. |
| [GetOperator](./getoperator/) | Ottiene e imposta il tipo di operatore della formattazione condizionale. |
| [SetOperator](./setoperator/) | Ottiene e imposta il tipo di operatore della formattazione condizionale. |
| [GetStopIfTrue](./getstopiftrue/) | True, nessuna regola con priorità inferiore può essere applicata a questa regola, quando questa regola restituisce true. Si applica solo per Excel 2007; |
| [SetStopIfTrue](./setstopiftrue/) | True, nessuna regola con priorità inferiore può essere applicata a questa regola, quando questa regola restituisce true. Si applica solo per Excel 2007; |
| [GetPriority](./getpriority/) | La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formattazione deve essere valutata e renderizzata. I valori numerici più bassi hanno priorità più alta rispetto ai valori numerici più alti, dove '1' è la priorità più alta. |
| [SetPriority](./setpriority/) | La priorità di questa regola di formattazione condizionale. Questo valore è usato per determinare quale formattazione deve essere valutata e renderizzata. I valori numerici più bassi hanno priorità più alta rispetto ai valori numerici più alti, dove '1' è la priorità più alta. |
| [GetStyle](./getstyle/) | Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente. |
| [SetStyle](./setstyle/) | Ottiene o imposta lo stile degli intervalli di celle formattate condizionalmente. |
| [GetType](./gettype/) | Ottiene e imposta se il tipo di formattazione condizionale è abilitato. |
| [SetType](./settype/) | Ottiene e imposta se il tipo di formattazione condizionale è abilitato. |
| [GetIconSet](./geticonset/) | Ottieni l'istanza "IconSet" della formattazione condizionale. Il tipo predefinito dell'istanza IconSet è TrafficLights31. Valido solo per type = IconSet. |
| [GetDataBar](./getdatabar/) | Ottieni l'istanza "DataBar" della formattazione condizionale. Il colore predefinito dell'istanza è blu. Valido solo per type = DataBar. |
| [GetColorScale](./getcolorscale/) | Ottieni l'istanza "ColorScale" della formattazione condizionale. L'istanza predefinita è una "green-yellow-red" 3ColorScale. Valido solo per type = ColorScale. |
| [GetTop10](./gettop10/) | Ottieni l'istanza "Top10" della formattazione condizionale. La regola predefinita dell'istanza evidenzia le celle i cui valori rientrano nella fascia dei primi 10. Valido solo per type = Top10. |
| [GetAboveAverage](./getaboveaverage/) | Ottieni l'istanza "AboveAverage" della formattazione condizionale. La regola predefinita dell'istanza evidenzia le celle che sono al di sopra della media per tutti i valori nell'intervallo. Valido solo per type = AboveAverage. |
| [GetText](./gettext/) | Il valore di testo in una regola di formattazione condizionale "text contains". Valido solo per type = containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null. |
| [SetText](./settext/) | Il valore di testo in una regola di formattazione condizionale "text contains". Valido solo per type = containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null. |
| [GetTimePeriod](./gettimeperiod/) | Il periodo di tempo applicabile in una regola di formattazione condizionale "date occurring". Valido solo per type = timePeriod. Il valore predefinito è TimePeriodType.Today. |
| [SetTimePeriod](./settimeperiod/) | Il periodo di tempo applicabile in una regola di formattazione condizionale "date occurring". Valido solo per type = timePeriod. Il valore predefinito è TimePeriodType.Today. |
