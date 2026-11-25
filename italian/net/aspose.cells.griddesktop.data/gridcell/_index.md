---
title: "Classe GridCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridDesktop.Data.GridCell. Rappresenta un oggetto cella"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Rappresenta un oggetto cella.

```csharp
public class GridCell
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Restituisce il valore booleano contenuto nella cella. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Restituisce il numero della colonna (basato su zero) della cella. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Restituisce il valore DateTime contenuto nella cella. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Restituisce il valore stringa formattato di questa cella. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Restituisce il valore double contenuto nella cella. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Restituisce il valore float contenuto nella cella. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Ottiene o imposta una formula della cella. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Indica se questa cella ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Ottiene e imposta la stringa HTML che contiene dati e alcune formattazioni in questa cella. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Restituisce il valore intero contenuto nella cella. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Ottiene il nome della cella. Ad esempio: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Indica se la cella è protetta. Se il valore è "true", l'utente non può modificare la cella tramite l'interfaccia utente. Questo attributo non ha nulla a che fare con la proprietà Style.CellLocked e non verrà salvato su file quando i dati della griglia vengono esportati. Il valore predefinito è "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Ottiene il numero di riga (basato su zero) della cella. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Restituisce il valore stringa contenuto nella cella. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Ottiene una copia dello stile della cella. Imposta lo stile per la cella. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | Restituisce il tipo di valore della cella, il significato può essere visto in GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Ottiene il valore contenuto in questa cella. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Ottiene l'oggetto foglio di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella formula. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Copia i dati da una cella di origine. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | Copia lo stile e imposta lo stile per la cella |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Ottiene il font della cella. Quando si cambia il font, è necessario invocare il metodo "SetFont" per impostare il font nella cella. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Ottiene il colore del font della cella. Quando si cambia il colore, è necessario invocare il metodo "SetFontColor" per impostare il colore del font nella cella. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Ottiene lo stile della cella. Quando si cambia lo stile, è necessario invocare il metodo "SetStyle" per impostare lo stile nella cella. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Ottiene la convalida applicata a questa cella. Se non impostata, restituisce null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Ottiene la larghezza del valore in unità di pixel. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Ottiene il foglio di lavoro genitore. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Verifica se una formula può valutare correttamente un risultato. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Rappresenta se la cella specificata contiene una formula. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Inserisce un valore booleano nella cella. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Inserisce un valore DateTime nella cella. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Inserisce un valore double nella cella. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Inserisce un valore intero nella cella. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Inserisce un valore oggetto nella cella.stesso di setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Inserisce un valore String nella cella. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dato, se appropriato. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Inserisce un valore nella cella; se appropriato, il valore sarà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Imposta il valore della cella con un valore stringa e imposta il formato della cella in base a questo valore. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Se il valore è una formula, questo metodo imposta il valore della cella come FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | Imposta il formato personalizzato, null o stringa vuota significa nessun formato personalizzato. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Imposta il carattere nella cella. Per migliorare le prestazioni, implementare il metodo "SetFont", non implementare la proprietà "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Imposta il colore del carattere nella cella. Per migliorare le prestazioni, implementare il metodo "SetFontColor", non implementare la proprietà "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Imposta la formula e il valore della formula. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | imposta il formato di visualizzazione di numeri e date |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Imposta lo stile nella cella. Per migliorare le prestazioni, implementare il metodo "SetStyle", non implementare la proprietà "Style". |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


