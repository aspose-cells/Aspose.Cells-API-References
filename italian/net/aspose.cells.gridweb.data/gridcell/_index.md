---
title: GridCell
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta un oggetto cella.
type: docs
weight: 150
url: /it/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Rappresenta un oggetto cella.

```csharp
public class GridCell
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Ottiene il valore booleano contenuto nella cella. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Ottiene il numero di colonna (in base zero) della cella. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Ottiene il valore DateTime contenuto nella cella. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Ottiene il valore della stringa formattata di questa cella. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Ottiene il valore double contenuto nella cella. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Ottiene il valore float contenuto nella cella. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Ottiene o imposta una formula diCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Ottiene e imposta la stringa html che contiene i dati e alcune formattazioni in questa cella. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Ottiene il valore intero contenuto nella cella. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Ottiene il nome della cella. Ad esempio: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Ottiene il numero di riga (in base zero) della cella. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Ottiene il valore della stringa contenuto nella cella. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Ottiene la copia dello stile della cella. imposta lo stile per la cella. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | restituisce il tipo di valore della cella, il significato può vedere GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Ottiene il valore contenuto in questa cella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella formula. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Copia i dati da una cella di origine. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | copia lo stile e imposta lo stile per la cella |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Crea un oggetto commento per una cella. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Crea un oggetto di convalida per una cella. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Ottieni oggetto commento su questa cella |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Ottiene la larghezza del valore in unità di pixel. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Verifica se una formula può valutare correttamente un risultato. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Rappresenta se la cella specificata contiene la formula. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Inserisce un valore booleano nella cella. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Inserisce un valore DateTime nella cella. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Inserisce un valore doppio nella cella. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Inserisce un valore int nella cella. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | Inserisce un valore oggetto nella cella.same di setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Inserisce un valore String nella cella. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dati, se appropriato. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Inserisce un valore nella cella, se appropriato il valore verrà convertito in un altro tipo di dati e il formato del numero della cella verrà reimpostato. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Imposta il valore della cella con un valore stringa e imposta il formato della cella in base a questo valore. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Rimuove l'oggetto commento dalla cella. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Rimuove l'oggetto di convalida della cella. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Imposta i bordi (in alto, in basso, a sinistra e a destra) per una cella, tutti i bordi hanno lo stesso stile di bordo. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | imposta il formato personalizzato, la stringa nulla o vuota significa nessun formato personalizzato. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Imposta la formula e il valore della formula. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | imposta il formato di visualizzazione di numeri e date |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
