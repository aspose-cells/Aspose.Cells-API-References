---
title: "Classe Cell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Cell. Incapsula l'oggetto che rappresenta una singola cella del Workbook"
type: docs
url: /it/net/aspose.cells/cell/
---
## Cell class

Incapsula l'oggetto che rappresenta una singola cella del Workbook.

```csharp
public class Cell
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Restituisce il valore booleano contenuto nella cella. |
| [Column](../../aspose.cells/cell/column/) { get; } | Restituisce il numero della colonna (basato su zero) della cella. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Restituisce il commento di questa cella. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella di formula. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Restituisce il valore DateTime contenuto nella cella. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Restituisce il valore stringa formattato di questa cella secondo lo stile di visualizzazione della cella. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Restituisce il valore double contenuto nella cella. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Restituisce e imposta l'immagine incorporata nella cella. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Restituisce il valore float contenuto nella cella. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Restituisce o imposta una formula della `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Restituisce la formula formattata per la lingua locale della cella. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Verifica se nella formula di questa cella è presente una funzione personalizzata (funzione non supportata). |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Indica se questa cella ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Restituisce e imposta la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Restituisce il valore intero contenuto nella cella. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Indica se la formula della cella è una formula array. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Indica che la formula della cella è una formula array ed è la prima cella dell'array. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Indica se impostare questa cella come casella di controllo. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Indica se la formula della cella è una formula array dinamica (true) o una formula array legacy (false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Verifica se il valore di questa cella è un errore. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Rappresenta se la cella specificata contiene una formula. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Indica se la formula della cella è una formula array. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Indica se questa cella fa parte di una formula di tabella. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Verifica se una cella fa parte di un intervallo unito o meno. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Indica se il valore di questa cella è numerico (int, double e datetime). |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Indica se la formula della cella è parte di una formula condivisa. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Indica se questa cella fa parte di una formula di tabella. |
| [Name](../../aspose.cells/cell/name/) { get; } | Ottiene il nome della cella. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Rappresenta il tipo di categoria della formattazione numerica di questa cella. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Ottiene un'istanza di [`Picture`](../../aspose.cells.drawing/picture/) che rappresenta l'immagine incorporata in questa cella o null se non esiste alcuna immagine incorporata per questa cella. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Ottiene o imposta una formula R1C1 della `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | Ottiene il numero di riga (basato su zero) della cella. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Ottiene l'indice di stile condiviso della cella nel pool di stili. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Ottiene il valore stringa contenuto nella cella. Se il tipo di questa cella è stringa, restituisce il valore stringa stesso. Per gli altri tipi di cella, verrà restituito il valore stringa formattato (formattato con lo stile specificato di questa cella). Il valore della cella formattato è lo stesso di quello che si ottiene da Excel copiando una cella come testo (ad esempio copiando la cella in un editor di testo o esportando in CSV). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Ottiene il valore della cella come stringa senza alcuna formattazione. |
| [Type](../../aspose.cells/cell/type/) { get; } | Rappresenta il tipo di valore della cella. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Ottiene/imposta il valore contenuto in questa cella. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Ottiene il foglio di lavoro genitore. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Calcola la formula della cella. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo della cella. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Copia i dati da una cella di origine. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Verifica se questo oggetto si riferisce alla stessa cella di un altro. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Ottiene l'intervallo di array se la formula della cella è una formula di matrice. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo della cella. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo della cella. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Ottieni il risultato della formattazione condizionale. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Ottiene tutte le celle il cui risultato calcolato dipende da questa cella. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Ottiene lo stile di visualizzazione di questa cella. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Ottiene lo stile di visualizzazione di questa cella. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Ottiene lo stile di visualizzazione di questa cella. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Ottiene le condizioni di formattazione che si applicano a questa cella. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Ottieni la formula di questa cella. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Funziona come funzione hash per un tipo particolare. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Ottiene l'altezza del valore in unità di pixel. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Ottiene la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Ottieni tutte le celle che fanno riferimento direttamente a questa cella e devono essere aggiornate quando questa cella viene modificata. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Ottieni tutte le celle che saranno aggiornate quando questa cella viene modificata. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Restituisce un oggetto [`Range`](../range/) che rappresenta un intervallo unito. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Ottiene tutti i riferimenti presenti nella formula di questa cella. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Ottiene tutti i precedenti (riferimento a celle nella cartella di lavoro corrente) utilizzati dalla formula di questa cella durante il calcolo. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Ottiene il valore ricco della cella. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Ottiene il valore stringa mediante una strategia di formattazione specifica. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Ottiene lo stile della cella. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | Se checkBorders è true, verifica se i bordi delle altre celle influenzeranno lo stile di questa cella. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Ottiene la tabella che contiene questa cella. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Ottiene la convalida applicata a questa cella. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Ottiene il valore di convalida applicato a questa cella. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Ottiene la larghezza del valore in unità di pixel. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Inserisce alcuni caratteri nella cella. Se la cella è formattata in rich text, questo metodo può mantenere la formattazione originale. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Indica se il valore stringa di questa cella è un testo formattato in rich text. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Inserisce un valore booleano nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Inserisce un valore DateTime nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Inserisce un valore double nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Inserisce un valore intero nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Inserisce un valore oggetto nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Inserisce un valore stringa nella cella. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dato, se appropriato. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Inserisce un valore nella cella; se appropriato, il valore sarà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Rimuove la formula di matrice. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Sostituisce il testo della cella con le opzioni. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Imposta una formula di matrice (formula di matrice legacy inserita tramite CTRL+SHIFT+ENTER in MS Excel) a un intervallo di celle. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Imposta una formula di matrice a un intervallo di celle. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Imposta una formula di matrice a un intervallo di celle. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Imposta una formula di matrice a un intervallo di celle. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Imposta il formato rich text della cella. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Imposta una formula di matrice dinamica e fa sì che la formula si espanda nelle celle vicine, se possibile. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Imposta una formula di matrice dinamica e fa sì che la formula si espanda nelle celle vicine, se possibile. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Imposta una formula di matrice dinamica e fa sì che la formula si espanda nelle celle vicine, se possibile. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Imposta la formula e il valore della formula. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Imposta formule condivise a un intervallo di celle. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Imposta formule condivise a un intervallo di celle. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Imposta una formula a un intervallo di celle. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Imposta formule condivise a un intervallo di celle. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Imposta lo stile della cella. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Applica la proprietà modificata dello stile alla cella. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Applica lo stile della cella in base ai flag. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Converti `Cell` in dati struct JSON. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Accedi alla raccolta di celle
            Cells cells = worksheet.Cells;

            // Inserisci una stringa in una cella
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Inserisci un intero in una cella
            cell = cells["B1"];
            cell.PutValue(12);

            // Inserisci un double in una cella
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Inserisci una formula in una cella
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Inserisci una formula combinata: "sum(average(b1,c1), b1)" nella cella b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Imposta lo stile di una cella
            Style style = cell.GetStyle();
            // Imposta il colore di sfondo
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Imposta il carattere di una cella
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


