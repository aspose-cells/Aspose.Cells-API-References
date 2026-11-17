---
title: "Classe Cell"
linktitle: "Cell"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Cell. Incapsula l'oggetto che rappresenta cell in Go."
type: docs
weight: 200
url: /it/go-cpp/cell/
---

## Cell class

Incapsula l'oggetto che rappresenta una singola cella di Workbook.

```go

type Cell struct  {
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
| [Calculate](./calculate/) | Calcola la formula della cella. |
| [GetWorksheet](./getworksheet/) | Ottiene il foglio di lavoro padre. |
| [PutValue_Bool](./putvalue_bool/) | Inserisce un valore booleano nella cella. |
| [PutValue_Int](./putvalue_int/) | Inserisce un valore intero nella cella. |
| [PutValue_Double](./putvalue_double/) | Inserisce un valore double nella cella. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Inserisce un valore nella cella; se opportuno, il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [PutValue_String_Bool](./putvalue_string_bool/) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dato se opportuno. |
| [PutValue_String](./putvalue_string/) | Inserisce un valore stringa nella cella. |
| [PutValue_Date](./putvalue_date/) | Inserisce un valore DateTime nella cella. |
| [PutValue_Object](./putvalue_object/) | Inserisce un valore oggetto nella cella. |
| [GetRow](./getrow/) | Ottiene il numero di riga (basato su zero) della cella. |
| [GetColumn](./getcolumn/) | Ottiene il numero di colonna (basato su zero) della cella. |
| [IsFormula](./isformula/) | Rappresenta se la cella specificata contiene una formula. |
| [GetHasCustomFunction](./gethascustomfunction/) | Verifica se nella formula di questa cella è presente una funzione personalizzata (funzione non supportata). |
| [GetType](./gettype/) | Rappresenta il tipo di valore della cella. |
| [GetName](./getname/) | Ottiene il nome della cella. |
| [IsErrorValue](./iserrorvalue/) | Verifica se il valore di questa cella è un errore. |
| [IsNumericValue](./isnumericvalue/) | Indica se il valore di questa cella è numerico (int, double e datetime). |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Ottiene il valore stringa secondo una strategia di formattazione specifica. |
| [GetStringValue](./getstringvalue/) | Ottiene il valore stringa contenuto nella cella. Se il tipo di questa cella è stringa, restituisce il valore stringa stesso. Per gli altri tipi di cella, verrà restituito il valore stringa formattato (formattato con lo stile specificato di questa cella). Il valore della cella formattato è lo stesso di quello che si ottiene da Excel copiando una cella come testo (ad esempio copiando la cella in un editor di testo o esportando in CSV). |
| [GetNumberCategoryType](./getnumbercategorytype/) | Rappresenta il tipo di categoria della formattazione numerica di questa cella. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | Ottiene il valore stringa formattato di questa cella secondo lo stile di visualizzazione della cella. |
| [GetIntValue](./getintvalue/) | Ottiene il valore intero contenuto nella cella. |
| [GetDoubleValue](./getdoublevalue/) | Ottiene il valore double contenuto nella cella. |
| [GetFloatValue](./getfloatvalue/) | Ottiene il valore float contenuto nella cella. |
| [GetDateTimeValue](./getdatetimevalue/) | Ottiene il valore DateTime contenuto nella cella. |
| [GetBoolValue](./getboolvalue/) | Ottiene il valore booleano contenuto nella cella. |
| [GetWidthOfValue](./getwidthofvalue/) | Ottiene la larghezza del valore in unità di pixel. |
| [GetHeightOfValue](./getheightofvalue/) | Ottiene l'altezza del valore in unità di pixel. |
| [GetDisplayStyle](./getdisplaystyle/) | Ottiene lo stile di visualizzazione di questa cella. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Ottiene lo stile di visualizzazione di questa cella. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Ottiene lo stile di visualizzazione di questa cella. |
| [GetFormatConditions](./getformatconditions/) | Ottiene le condizioni di formattazione che si applicano a questa cella. |
| [GetStyle](./getstyle/) | Ottiene lo stile della cella. |
| [GetStyle_Bool](./getstyle_bool/) | Se checkBorders è true, verifica se i bordi delle altre celle influenzeranno lo stile di questa cella. |
| [SetStyle_Style](./setstyle_style/) | Imposta lo stile della cella. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Applica la proprietà modificata dello stile alla cella. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Applica lo stile della cella in base ai flag. |
| [GetHasCustomStyle](./gethascustomstyle/) | Indica se questa cella ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente). |
| [GetSharedStyleIndex](./getsharedstyleindex/) | Ottiene l'indice di stile condiviso della cella nel pool di stili. |
| [GetFormula](./getformula/) | Ottiene o imposta una formula della cella. |
| [SetFormula_String](./setformula_string/) | Ottiene o imposta una formula della cella. |
| [GetFormulaLocal](./getformulalocal/) | Ottieni la formula formattata per la lingua della cella. |
| [SetFormulaLocal](./setformulalocal/) | Ottieni la formula formattata per la lingua della cella. |
| [GetR1C1Formula](./getr1c1formula/) | Ottiene o imposta una formula R1C1 della cella. |
| [SetR1C1Formula](./setr1c1formula/) | Ottiene o imposta una formula R1C1 della cella. |
| [SetFormula_String_Object](./setformula_string_object/) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | Ottieni la formula di questa cella. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Imposta una formula array (formula array legacy inserita tramite CTRL+SHIFT+ENTER in MS Excel) a un intervallo di celle. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Imposta una formula array a un intervallo di celle. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Imposta una formula array a un intervallo di celle. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Imposta formule condivise a un intervallo di celle. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Imposta formule condivise a un intervallo di celle. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Imposta formule condivise a un intervallo di celle. |
| [GetContainsExternalLink](./getcontainsexternallink/) | Indica se questa cella contiene un collegamento esterno. Valido solo quando la cella è una cella di formula. |
| [GetPrecedents](./getprecedents/) | Ottiene tutti i riferimenti presenti nella formula di questa cella. |
| [GetDependents](./getdependents/) | Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | Ottiene tutti i precedenti (riferimenti a celle nella cartella di lavoro corrente) usati dalla formula di questa cella durante il calcolo. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Ottiene tutte le celle il cui risultato calcolato dipende da questa cella. |
| [IsArrayHeader](./isarrayheader/) | Indica che la formula della cella è una formula array e che è la prima cella dell'array. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | Indica se la formula della cella è una formula array dinamica (true) o una formula array legacy (false). |
| [GetArrayRange](./getarrayrange/) | Ottiene l'intervallo array se la formula della cella è una formula array. |
| [IsArrayFormula](./isarrayformula/) | Indica se la formula della cella è una formula array. |
| [IsSharedFormula](./issharedformula/) | Indica se la formula della cella fa parte di una formula condivisa. |
| [IsTableFormula](./istableformula/) | Indica se questa cella fa parte di una formula tabella. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Imposta una formula array dinamica e fa sì che la formula si estenda alle celle vicine, se possibile. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Imposta una formula array dinamica e fa sì che la formula si estenda alle celle vicine, se possibile. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Imposta una formula array dinamica e fa sì che la formula si estenda alle celle vicine, se possibile. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella. |
| [RemoveArrayFormula](./removearrayformula/) | Rimuovi la formula array. |
| [Copy](./copy/) | Copia i dati da una cella di origine. |
| [GetValue](./getvalue/) | Ottiene/imposta il valore contenuto in questa cella. |
| [SetValue](./setvalue/) | Ottiene/imposta il valore contenuto in questa cella. |
| [IsStyleSet](./isstyleset/) | Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito. |
| [Characters](./characters/) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo della cella. |
| [Replace](./replace/) | Sostituisce il testo della cella con opzioni. |
| [InsertText](./inserttext/) | Inserisce alcuni caratteri nella cella. Se la cella è formattata in rich, questo metodo può mantenere la formattazione originale. |
| [IsRichText](./isrichtext/) | Indica se il valore stringa di questa cella è un testo formattato in rich. |
| [GetCharacters](./getcharacters/) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella. |
| [GetCharacters_Bool](./getcharacters_bool/) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella. |
| [SetCharacters](./setcharacters/) | Imposta il formato di testo ricco della cella. |
| [IsMerged](./ismerged/) | Verifica se una cella fa parte di un intervallo unito o meno. |
| [GetMergedRange](./getmergedrange/) | Restituisce un oggetto Range che rappresenta un intervallo unito. |
| [GetComment](./getcomment/) | Ottiene il commento di questa cella. |
| [GetHtmlString](./gethtmlstring/) | Ottiene e imposta la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [SetHtmlString](./sethtmlstring/) | Ottiene e imposta la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | Ottiene la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [ToString](./tostring/) | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |
| [ToJson](./tojson/) | Converti Cell in dati strutturati JSON. |
| [Equals_Object](./equals_object/) | Verifica se questo oggetto si riferisce alla stessa cella di un altro. |
| [GetHashCode](./gethashcode/) | Funziona come funzione hash per un tipo particolare. |
| [Equals_Cell](./equals_cell/) | Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | Ottieni il risultato della formattazione condizionale. |
| [GetValidation](./getvalidation/) | Ottiene la convalida applicata a questa cella. |
| [GetValidationValue](./getvalidationvalue/) | Ottiene il valore della convalida applicata a questa cella. |
| [GetTable](./gettable/) | Ottiene la tabella che contiene questa cella. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | Indica se impostare questa cella come casella di controllo. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | Indica se impostare questa cella come casella di controllo. |
| [GetRichValue](./getrichvalue/) | Ottiene il valore ricco della cella. |
| [GetEmbeddedImage](./getembeddedimage/) | Ottiene e imposta l'immagine incorporata nella cella. |
| [SetEmbeddedImage](./setembeddedimage/) | Ottiene e imposta l'immagine incorporata nella cella. |
| [GetPicture](./getpicture/) | Ottiene un'istanza di Aspose.Cells.Drawing.Picture per rappresentare l'immagine incorporata in questa cella o null se non esiste alcuna immagine incorporata per questa cella. |
|[Dispose](./dispose/) |  | 
