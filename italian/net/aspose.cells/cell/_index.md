---
title: Cell
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta una singola cella della cartella di lavoro.
type: docs
weight: 230
url: /it/net/aspose.cells/cell/
---
## Cell class

Incapsula l'oggetto che rappresenta una singola cella della cartella di lavoro.

```csharp
public class Cell
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Ottiene il valore booleano contenuto nella cella. |
| [Column](../../aspose.cells/cell/column) { get; } | Ottiene il numero di colonna (in base zero) della cella. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Ottiene il commento di questa cella. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella formula. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Ottiene il valore DateTime contenuto nella cella. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Ottiene il valore della stringa formattata di questa cella in base allo stile di visualizzazione della cella. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Ottiene il valore double contenuto nella cella. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Ottiene il valore float contenuto nella cella. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Ottiene o imposta una formula di[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Ottieni la formula formattata per le impostazioni locali della cella. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Ottiene e imposta la stringa html che contiene dati e alcuni formati in questa cella. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Ottiene il valore intero contenuto nella cella. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Indica se la formula della cella è una formula di matrice. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Indica che la formula della cella è e la formula della matrice ed è la prima cella della matrice. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Verifica se il valore di questa cella è un errore. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Rappresenta se la cella specificata contiene la formula. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Verifica se una cella fa parte di un intervallo unito o meno. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Indica se il valore interno di questa cella è numerico(int, double e datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Indica se la formula della cella fa parte della formula condivisa. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Indica se questa cella fa parte della formula della tabella. |
| [Name](../../aspose.cells/cell/name) { get; } | Ottiene il nome della cella. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Rappresenta il tipo di categoria della formattazione del numero di questa cella. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Ottiene o imposta una formula R1C1 di[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | Ottiene il numero di riga (in base zero) della cella. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Ottiene l'indice di stile condiviso della cella nel pool di stili. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Ottiene il valore della stringa contenuto nella cella. Se il tipo di questa cella è una stringa, restituisci il valore della stringa stessa. Per altri tipi di cella, verrà restituito il valore della stringa formattata (formattata con lo stile specificato di questa cella). Il valore della cella formattata è uguale a quello che hai può ottenere da Excel durante la copia di una cella come testo (come copia della cella nell'editor di testo o esportazione in CSV). |
| [Type](../../aspose.cells/cell/type) { get; } | Rappresenta il tipo di valore della cella. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Ottiene il valore contenuto in questa cella. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Ottiene il foglio di lavoro principale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Calcola la formula della cella. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Restituisce un oggetto Caratteri che rappresenta un intervallo di caratteri all'interno del testo della cella. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Copia i dati da una cella di origine. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Verifica se questo oggetto fa riferimento alla stessa cella con un altro oggetto cella. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Verifica se questo oggetto fa riferimento alla stessa cella con un'altra. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Ottiene l'intervallo di matrice se la formula della cella è una formula di matrice. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Ottieni il risultato della formattazione condizionale. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Ottiene tutte le celle il cui risultato calcolato dipende da questa cella. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Ottiene lo stile di visualizzazione della cella. Se questa cella è influenzata anche da altre impostazioni come formattazione condizionale, oggetti elenco e così via, lo stile di visualizzazione potrebbe essere diverso da cell.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Ottiene lo stile di visualizzazione della cella. Se la cella è formattata condizionale, lo stile di visualizzazione non è lo stesso della cella.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Ottiene le condizioni di formato che si applicano a questa cella. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Ottieni la formula di questa cella. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Serve come funzione hash per un tipo particolare. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Ottiene l'altezza del valore in unità di pixel. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Ottiene la stringa html che contiene dati e alcuni formati in questa cella. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Restituisce a[`Range`](../range) oggetto che rappresenta un intervallo unito. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Ottiene tutti i riferimenti che appaiono nella formula di questa cella. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Ottiene tutti i precedenti (riferimento alle celle nella cartella di lavoro corrente) utilizzati dalla formula di questa cella durante il calcolo. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Ottiene il valore della stringa in base a una specifica strategia formattata. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Ottiene lo stile della cella. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | Se checkBorders è vero, controlla se i bordi di altre celle influiranno sullo stile di questa cella. |
| [GetTable](../../aspose.cells/cell/gettable)() | Ottiene la tabella che contiene questa cella. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Ottiene la convalida applicata a questa cella. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Ottiene il valore di convalida applicato a questa cella. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Ottiene la larghezza del valore in unità di pixel. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Indica se il valore della stringa di cella è un testo RTF. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Inserisce un valore booleano nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Inserisce un valore DateTime nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Inserisce un valore doppio nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Inserisce un valore intero nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Inserisce un valore oggetto nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Inserisce un valore stringa nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dati, se appropriato. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Inserisce un valore nella cella, se appropriato il valore verrà convertito in un altro tipo di dati e il formato del numero della cella verrà reimpostato. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Rimuovi formula matrice. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Imposta una formula di matrice (formula di matrice legacy immessa tramite CTRL+MAIUSC+INVIO in ms excel) su un intervallo di celle. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Imposta una formula di matrice su un intervallo di celle. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Imposta una formula di matrice su un intervallo di celle. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Imposta il formato RTF della cella. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Imposta la formula della matrice dinamica e, se possibile, la formula si riversa nelle celle adiacenti. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Imposta la formula della matrice dinamica e, se possibile, la formula si riversa nelle celle adiacenti. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Imposta la formula e il valore della formula. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Imposta la formula e il valore della formula. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Imposta una formula su un intervallo di celle. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Imposta una formula su un intervallo di celle. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Imposta una formula su un intervallo di celle. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Imposta lo stile della cella. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Applica lo stile della cella. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Applica lo stile della cella. |
| override [ToString](../../aspose.cells/cell/tostring)() | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |

### Esempi

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Inserisce una stringa in una cella
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
//Inserisce un numero intero in una cella
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

//Metti un doppio in una cella
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

//Inserisce una formula in una cella
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Inserisci una formula combinata: "sum(average(b1,c1), b1)" nella cella in b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

//Imposta lo stile di una cella
Style style = cell.GetStyle();
//Imposta il colore di sfondo
style.BackgroundColor = Color.Yellow;
//Imposta il formato di una cella
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Metti una stringa in una cella
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
//Inserisce un numero intero in una cella
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

//Metti un doppio in una cella
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

//Inserisce una formula in una cella
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Inserisci una formula combinata: "sum(average(b1,c1), b1)" nella cella in b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
//Imposta lo stile di una cella
Dim style as Style = cell.GetStyle()

//Imposta il colore di sfondo
style.BackgroundColor = Color.Yellow
//Imposta il carattere di una cella
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
