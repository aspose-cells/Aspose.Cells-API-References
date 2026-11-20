---
title: "Cella"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta una singola cella del Workbook."
type: docs
url: /it/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Incapsula l'oggetto che rappresenta una singola cella del Workbook.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Calcola la formula della cella. |
| [characters(int startIndex, int length)](#characters-int-int-) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo della cella. |
| [containsExternalLink()](#containsExternalLink--) | Indica se questa cella contiene un collegamento esterno. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Copia i dati da una cella di origine. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella. |
| [equals(Object obj)](#equals-java.lang.Object-) | Verifica se questo oggetto si riferisce alla stessa cella di un altro. |
| [getArrayRange()](#getArrayRange--) | Ottiene l'intervallo di matrice se la formula della cella è una formula di matrice. |
| [getBoolValue()](#getBoolValue--) | Ottiene il valore booleano contenuto nella cella. |
| [getCharacters()](#getCharacters--) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ottiene il numero della colonna (basato su zero) della cella. |
| [getComment()](#getComment--) | Ottiene il commento di questa cella. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Ottieni il risultato della formattazione condizionale. |
| [getDateTimeValue()](#getDateTimeValue--) | Ottiene il valore DateTime contenuto nella cella. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Ottiene tutte le celle il cui risultato calcolato dipende da questa cella. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Ottiene il valore stringa formattato di questa cella secondo lo stile di visualizzazione della cella. |
| [getDisplayStyle()](#getDisplayStyle--) | Ottiene lo stile di visualizzazione di questa cella. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Ottiene lo stile di visualizzazione di questa cella. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Ottiene lo stile di visualizzazione di questa cella. |
| [getDoubleValue()](#getDoubleValue--) | Ottiene il valore double contenuto nella cella. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Ottiene l'immagine incorporata nella cella. |
| [getFloatValue()](#getFloatValue--) | Ottiene il valore float contenuto nella cella. |
| [getFormatConditions()](#getFormatConditions--) | Ottiene le condizioni di formattazione che si applicano a questa cella. |
| [getFormula()](#getFormula--) | Ottiene una formula della [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Ottieni la formula di questa cella. |
| [getFormulaLocal()](#getFormulaLocal--) | Ottieni la formula formattata in base alla locale della cella. |
| [getHeightOfValue()](#getHeightOfValue--) | Restituisce l'altezza del valore in unità di pixel. |
| [getHtmlString()](#getHtmlString--) | Restituisce la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Restituisce la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [getIntValue()](#getIntValue--) | Restituisce il valore intero contenuto nella cella. |
| [getLeafs()](#getLeafs--) | Ottieni tutte le celle che fanno riferimento a questa cella direttamente e devono essere aggiornate quando questa cella viene modificata. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Ottieni tutte le celle che saranno aggiornate quando questa cella viene modificata. |
| [getMergedRange()](#getMergedRange--) | Restituisce un oggetto [Range](../../com.aspose.cells/range) che rappresenta un intervallo unito. |
| [getName()](#getName--) | Restituisce il nome della cella. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Rappresenta il tipo di categoria della formattazione numerica di questa cella. |
| [getPicture()](#getPicture--) | Restituisce un'istanza [Picture](../../com.aspose.cells/picture) per rappresentare l'immagine incorporata in questa cella o null se non è presente alcuna immagine incorporata per questa cella. |
| [getPrecedents()](#getPrecedents--) | Restituisce tutti i riferimenti presenti nella formula di questa cella. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Restituisce tutti i precedenti (riferimenti a celle nella cartella di lavoro corrente) utilizzati dalla formula di questa cella durante il calcolo. |
| [getR1C1Formula()](#getR1C1Formula--) | Restituisce una formula R1C1 della [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | Restituisce il valore ricco della cella. |
| [getRow()](#getRow--) | Restituisce il numero di riga (basato su zero) della cella. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Restituisce l'indice di stile condiviso della cella nel pool di stili. |
| [getStringValue()](#getStringValue--) | Restituisce il valore stringa contenuto nella cella. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Restituisce il valore stringa secondo una strategia di formattazione specifica. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Restituisce il valore della cella come stringa senza alcuna formattazione. |
| [getStyle()](#getStyle--) | Restituisce lo stile della cella. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | Se checkBorders è true, verifica se i bordi di altre celle influenzeranno lo stile di questa cella. |
| [getTable()](#getTable--) | Restituisce la tabella che contiene questa cella. |
| [getType()](#getType--) | Rappresenta il tipo di valore della cella. |
| [getValidation()](#getValidation--) | Restituisce la convalida applicata a questa cella. |
| [getValidationValue()](#getValidationValue--) | Restituisce il valore della convalida applicata a questa cella. |
| [getValue()](#getValue--) | Restituisce il valore contenuto in questa cella. |
| [getWidthOfValue()](#getWidthOfValue--) | Restituisce la larghezza del valore in unità di pixel. |
| [getWorksheet()](#getWorksheet--) | Restituisce il foglio di lavoro genitore. |
| [hasCustomFunction()](#hasCustomFunction--) | Verifica se nella formula di questa cella è presente una funzione personalizzata (funzione non supportata). |
| [hasCustomStyle()](#hasCustomStyle--) | Indica se questa cella ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente). |
| [hashCode()](#hashCode--) | Funziona come funzione hash per un tipo specifico. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Inserisce alcuni caratteri nella cella. |
| [isArrayFormula()](#isArrayFormula--) | Indica se la formula della cella è una formula array. |
| [isArrayHeader()](#isArrayHeader--) | Indica che la formula della cella è una formula array e che è la prima cella dell'array. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Indica se questa cella è impostata come casella di controllo. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Indica se la formula della cella è una formula array dinamica (true) o una formula array legacy (false). |
| [isErrorValue()](#isErrorValue--) | Verifica se il valore di questa cella è un errore. |
| [isFormula()](#isFormula--) | Rappresenta se la cella specificata contiene una formula. |
| [isInArray()](#isInArray--) | Indica se la formula della cella è una formula array. |
| [isInTable()](#isInTable--) | Indica se questa cella fa parte di una formula di tabella. |
| [isMerged()](#isMerged--) | Verifica se una cella fa parte di un intervallo unito o meno. |
| [isNumericValue()](#isNumericValue--) | Indica se il valore di questa cella è numerico (int, double e datetime). |
| [isRichText()](#isRichText--) | Indica se il valore stringa di questa cella è un testo formattato riccamente. |
| [isSharedFormula()](#isSharedFormula--) | Indica se la formula della cella fa parte di una formula condivisa. |
| [isStyleSet()](#isStyleSet--) | Indica se lo stile della cella è impostato. |
| [isTableFormula()](#isTableFormula--) | Indica se questa cella fa parte di una formula di tabella. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Inserisce un valore booleano nella cella. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Inserisce un valore DateTime nella cella. |
| [putValue(double doubleValue)](#putValue-double-) | Inserisce un valore double nella cella. |
| [putValue(int intValue)](#putValue-int-) | Inserisce un valore intero nella cella. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Inserisce un valore oggetto nella cella. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Inserisce un valore stringa nella cella. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dati, se appropriato. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Inserisce un valore nella cella; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Rimuove la formula di matrice. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Sostituisce il testo della cella con opzioni. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Imposta una formula di matrice (formula di matrice legacy inserita tramite CTRL+SHIFT+ENTER in MS Excel) a un intervallo di celle. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Imposta una formula di matrice a un intervallo di celle. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Imposta una formula di matrice a un intervallo di celle. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Imposta una formula di matrice a un intervallo di celle. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Imposta il formato di testo avanzato della cella. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Indica se questa cella è impostata come casella di controllo. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Imposta una formula di matrice dinamica e fa sì che la formula si estenda alle celle adiacenti, se possibile. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Imposta una formula di matrice dinamica e fa sì che la formula si estenda alle celle adiacenti, se possibile. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Imposta una formula di matrice dinamica e fa sì che la formula si estenda alle celle adiacenti, se possibile. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Imposta l'immagine incorporata nella cella. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Imposta una formula della [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Imposta la formula e il valore della formula. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Imposta la formula e il valore (risultato calcolato) della formula. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Ottieni la formula formattata in base alla locale della cella. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Imposta la stringa HTML che contiene dati e alcuni formati in questa cella. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Imposta una formula R1C1 della [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Imposta formule condivise a un intervallo di celle. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Imposta una formula a un intervallo di celle. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Imposta formule condivise a un intervallo di celle. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Imposta formule condivise a un intervallo di celle. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Imposta lo stile della cella. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Applica la proprietà modificata dello stile alla cella. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applica lo stile della cella in base ai flag. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta il valore contenuto in questa cella. |
| [toJson()](#toJson--) | Converti la [Cell](../../com.aspose.cells/cell) in dati struct JSON. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Calcola la formula della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per il calcolo |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo della cella.

**Remarks**

Questo metodo funziona solo su celle con valore stringa.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice dell'inizio del carattere. |
| length | int | Il numero di caratteri. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella di formula.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Copia i dati da una cella di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Oggetto [Cell](../../com.aspose.cells/cell) di origine. |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | un altro oggetto cella |

**Returns:**
boolean - true se due oggetti cella si riferiscono alla stessa cella.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Verifica se questo oggetto si riferisce alla stessa cella di un altro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | un altro oggetto |

**Returns:**
boolean - true se due oggetti si riferiscono alla stessa cella.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Ottiene l'intervallo di matrice se la formula della cella è una formula di matrice.

**Remarks**

Si applica solo quando la formula della cella è una formula array.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Ottiene il valore booleano contenuto nella cella.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella.

**Returns:**
com.aspose.cells.FontSetting[] - Tutti gli oggetti Characters
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flag | boolean | Indica se applicare lo stile tabella alla cella se la cella è nella tabella. |

**Returns:**
com.aspose.cells.FontSetting[] - Tutti gli oggetti Characters
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Ottiene il numero della colonna (basato su zero) della cella.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


Ottiene il commento di questa cella.

**Remarks**

Se non esiste alcun commento applicato alla cella, restituisce null.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Ottieni il risultato della formattazione condizionale.

**Remarks**

Restituisce null se non è applicata alcuna formattazione condizionale a questa cella,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Ottiene il valore DateTime contenuto nella cella.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAll | boolean | Indica se controllare le formule in altri fogli di lavoro. |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Ottiene tutte le celle il cui risultato calcolato dipende da questa cella.

**Remarks**

Per utilizzare questo metodo, assicurati che la cartella di lavoro sia impostata con valore true per [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) e sia stata completamente calcolata con questa impostazione. Se non esiste alcun riferimento di formula a questa cella, verrà restituito null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| recursive | boolean | Indica se restituire quei dipendenti che non fanno riferimento a questa cella direttamente ma fanno riferimento ad altre foglie di questa cella. |

**Returns:**
java.util.Iterator - Enumeratore per elencare tutti i dipendenti (oggetti Cell)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Ottiene il valore stringa formattato di questa cella secondo lo stile di visualizzazione della cella.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Ottiene lo stile di visualizzazione di questa cella.

**Remarks**

Stesso utilizzo di [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) per [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). Cioè, questo metodo verificherà e regolerà i bordi superiore/inferiore/sinistro/destro di questa cella in base allo stile ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) delle celle adiacenti, ma non controllerà le celle unite e non controllerà lo stile di visualizzazione delle celle adiacenti.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Ottiene lo stile di visualizzazione di questa cella.

**Remarks**

Se il flag specificato è false, allora è equivalente a [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). Altrimenti è equivalente all'utilizzo di [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) per [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| includeMergedBorders | boolean | Indica se controllare i bordi delle celle unite. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Ottiene lo stile di visualizzazione di questa cella.

**Remarks**

Se questa cella è anche influenzata da altre impostazioni come la formattazione condizionale, gli oggetti elenco, ecc., lo stile di visualizzazione potrebbe differire da [getStyle()](../../com.aspose.cells/cell\#getStyle--).

Per i flag di regolazione dei bordi in base alle celle adiacenti, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) indicano se controllare e combinare i bordi inferiore/superiore/destro/sinistro delle celle sinistra/destra/sopra/sotto adiacenti a questa.

Per motivi di prestazioni e compatibilità, alcuni enum sono usati per indicare operazioni speciali:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Nota bene, il controllo dei bordi/stili delle celle adiacenti, soprattutto gli stili di visualizzazione, è un processo che richiede tempo. Se non è necessario ottenere i bordi per lo stile restituito, utilizzare [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) per disabilitare il processo delle celle adiacenti migliorerà le prestazioni. Quando si ottengono i bordi delle celle adiacenti dagli stili definiti solo su quelle celle (senza impostare [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)), le prestazioni possono essere migliori perché anche il controllo dello stile di visualizzazione di una cella richiede tempo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indica quali bordi devono essere controllati e regolati in base ai bordi delle celle adiacenti. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Ottiene il valore double contenuto nella cella.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Ottiene l'immagine incorporata nella cella.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Ottiene il valore float contenuto nella cella.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Ottiene le condizioni di formattazione che si applicano a questa cella.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - Restituisce l'oggetto [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Ottiene una formula della [Cell](../../com.aspose.cells/cell).

**Remarks**

Una stringa di formula inizia sempre con un segno di uguale (=). E si prega di utilizzare sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


Ottieni la formula di questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - la formula di questa cella.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Ottieni la formula formattata in base alla locale della cella.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Restituisce l'altezza del valore in unità di pixel.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Restituisce la stringa HTML che contiene dati e alcuni formati in questa cella.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Restituisce la stringa HTML che contiene dati e alcuni formati in questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| html5 | boolean | Indica se il valore è compatibile con html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Restituisce il valore intero contenuto nella cella.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Ottieni tutte le celle che fanno riferimento a questa cella direttamente e devono essere aggiornate quando questa cella viene modificata.

**Remarks**

NOTE: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.GetDependentsInCalculation(bool) per ottenere tutti i dipendenti nella catena di calcolo. Questa proprietà sarà rimossa 12 mesi dopo a partire da maggio 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
java.util.Iterator - Enumeratore per elencare tutti i dipendenti (Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Ottieni tutte le celle che saranno aggiornate quando questa cella viene modificata.

**Remarks**

NOTE: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.GetDependentsInCalculation(bool) per ottenere tutti i dipendenti nella catena di calcolo. Questa proprietà sarà rimossa 12 mesi dopo a partire da maggio 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| recursive | boolean | Restituisce i fogli che non fanno riferimento a questa cella direttamente ma fanno riferimento ad altri fogli di questa cella. |

**Returns:**
java.util.Iterator - Enumeratore per elencare tutti i dipendenti (Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Restituisce un oggetto [Range](../../com.aspose.cells/range) che rappresenta un intervallo unito.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Restituisce il nome della cella.

**Remarks**

Un nome di cella include la sua lettera di colonna e il numero di riga. Per esempio, il nome di una cella nella riga 0 e colonna 0 è A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Rappresenta il tipo di categoria della formattazione numerica di questa cella.

Vedi [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

Quando il modello di formattazione della cella è combinato con i modelli di formattazione condizionale, il tipo restituito corrisponde alla parte utilizzata per il valore corrente di questa cella. Per esempio, se il modello di formattazione per questa cella è "\\#,\\#\\#0;(\\#,\\#\\#0);"-";@", allora quando il valore della cella è numerico e diverso da 0, il tipo restituito è [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\\#NUMBER); Quando il valore della cella è 0 o non è un valore numerico, il tipo restituito è [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Restituisce un'istanza [Picture](../../com.aspose.cells/picture) per rappresentare l'immagine incorporata in questa cella o null se non è presente alcuna immagine incorporata per questa cella.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Restituisce tutti i riferimenti presenti nella formula di questa cella.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


Restituisce tutti i precedenti (riferimenti a celle nella cartella di lavoro corrente) utilizzati dalla formula di questa cella durante il calcolo.

**Remarks**

Questo metodo può funzionare solo nella situazione in cui [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\\#getEnableCalculationChain--) è true per la cartella di lavoro e la cartella di lavoro è stata completamente calcolata. Se questa cella non è una formula o non fa riferimento a nessun'altra cella, verrà restituito null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator - Enumeratore per elencare tutti i riferimenti (ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


Restituisce una formula R1C1 della [Cell](../../com.aspose.cells/cell).

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Restituisce il valore ricco della cella.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce il numero di riga (basato su zero) della cella.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Restituisce l'indice di stile condiviso della cella nel pool di stili.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Ottiene il valore stringa contenuto nella cella. Se il tipo di questa cella è string, restituisce il valore stringa stesso. Per altri tipi di cella, verrà restituito il valore stringa formattato (formattato con lo stile specificato di questa cella). Il valore della cella formattato è lo stesso di quello che si può ottenere da Excel copiando una cella come testo (ad esempio copiando la cella in un editor di testo o esportando in CSV).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Restituisce il valore stringa secondo una strategia di formattazione specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). La strategia formattata. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Restituisce il valore della cella come stringa senza alcuna formattazione.

**Remarks**

NOTE: Questo metodo è ora obsoleto. Invece, l'utente dovrebbe ottenere l'oggetto valore e formattarlo in base al tipo di valore e ai requisiti specifici. Questa proprietà sarà rimossa 12 mesi dopo a partire da dicembre 2020. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Restituisce lo stile della cella.

**Remarks**

Per modificare lo stile della cella, si prega di chiamare il metodo Cell.SetStyle() dopo aver modificato l'oggetto stile restituito. Questo metodo è lo stesso di [getStyle(boolean)](../../com.aspose.cells/cell\\#getStyle-boolean-) con valore true per il parametro.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


Se checkBorders è true, verifica se i bordi di altre celle influenzeranno lo stile di questa cella.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| checkBorders | boolean | Controlla i bordi delle altre celle |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Restituisce la tabella che contiene questa cella.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo di valore della cella.

Vedi [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Restituisce la convalida applicata a questa cella.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Restituisce il valore della convalida applicata a questa cella.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


Restituisce il valore contenuto in questa cella.

**Remarks**

Tipo possibile:

null,

Boolean,

DateTime,

Double,

Integer

String.

Per un valore int, può essere restituito come un oggetto Integer o un oggetto Double. E non c'è alcuna garanzia che il valore restituito rimanga sempre dello stesso tipo di oggetto.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Restituisce la larghezza del valore in unità di pixel.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Restituisce il foglio di lavoro genitore.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Verifica se nella formula di questa cella è presente una funzione personalizzata (funzione non supportata).

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indica se questa cella ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funziona come funzione hash per un tipo specifico.

**Returns:**
int - Un codice hash per l'oggetto Cell corrente.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Inserisci alcuni caratteri nella cella. Se la cella è formattata in modo avanzato, questo metodo può mantenere la formattazione originale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice. |
| testo | java.lang.String | Testo inserito. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indica se la formula della cella è una formula array.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Indica che la formula della cella è una formula array e che è la prima cella dell'array.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Indica se questa cella è impostata come casella di controllo.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Indica se la formula della cella è una formula array dinamica (true) o una formula array legacy (false).

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Verifica se il valore di questa cella è un errore.

**Remarks**

Vale anche per le celle di formula per verificare se il risultato calcolato è un errore.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Rappresenta se la cella specificata contiene una formula.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Indica se la formula della cella è una formula array.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.IsArrayFormula per verificare se la formula della cella è una formula array. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2018. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Indica se questa cella fa parte di una formula di tabella.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.IsTableFormula per verificare se la formula della cella fa parte di una formula tabella. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2018. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Verifica se una cella fa parte di un intervallo unito o meno.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Indica se il valore di questa cella è numerico (int, double e datetime).

**Remarks**

Vale anche per le celle di formula per verificare il risultato calcolato

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Indica se il valore stringa di questa cella è un testo formattato riccamente.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Indica se la formula della cella fa parte di una formula condivisa.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Indica se questa cella fa parte di una formula di tabella.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


Inserisce un valore booleano nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Inserisce un valore DateTime nella cella.

**Remarks**

Impostare un valore DateTime per una cella non significa che la cella verrà formattata automaticamente come data/ora. Il valore DateTime viene mantenuto come valore numerico nel modello dati sia di MS Excel sia di Aspose.Cells. Se il valore numerico verrà interpretato come valore numerico stesso o come data/ora dipende dal formato numerico applicato a questa cella. Se questa cella non è stata formattata come data/ora, verrà visualizzata come valore numerico anche se l'input è un DateTime.

**Example**

Questo esempio mostra come impostare un valore DateTime in una cella e farlo visualizzare come data/ora.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Valore di input |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Inserisce un valore double nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleValue | double | Valore di input |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Inserisce un valore intero nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intValue | int | Valore di input |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Inserisce un valore oggetto nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objectValue | java.lang.Object | valore di input |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Inserisce un valore stringa nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dati, se appropriato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input |
| isConverted | boolean | True: convertito in un altro tipo di dato se appropriato. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Inserisce un valore nella cella; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input |
| isConverted | boolean | True: convertito in un altro tipo di dato se appropriato. |
| setStyle | boolean | True: imposta il formato numerico nello stile della cella durante la conversione in un altro tipo di dato |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Rimuove la formula di matrice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| leaveNormalFormula | boolean | True rappresenta la conversione della formula array in una formula normale. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Sostituisce il testo della cella con opzioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValue | java.lang.String | Valore stringa da sostituire |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Le opzioni di sostituzione |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Imposta una formula di matrice (formula di matrice legacy inserita tramite CTRL+SHIFT+ENTER in MS Excel) a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formula array. |
| rowNumber | int | Numero di righe per popolare il risultato della formula array. |
| columnNumber | int | Numero di colonne per popolare il risultato della formula di matrice. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Imposta una formula di matrice a un intervallo di celle.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2019. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formula array. |
| rowNumber | int | Numero di righe per popolare il risultato della formula array. |
| columnNumber | int | Numero di colonne per popolare il risultato della formula di matrice. |
| isR1C1 | boolean | se la formula è una formula R1C1 |
| isLocal | boolean | se la formula è formattata secondo la locale |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Imposta una formula di matrice a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formula array. |
| rowNumber | int | Numero di righe per popolare il risultato della formula array. |
| columnNumber | int | Numero di colonne per popolare il risultato della formula di matrice. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Imposta una formula di matrice a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | Formula array. |
| rowNumber | int | Numero di righe per popolare il risultato della formula array. |
| columnNumber | int | Numero di colonne per popolare il risultato della formula di matrice. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |
| valori | java.lang.Object[][] | valori per quelle celle con la formula di matrice fornita |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Imposta il formato di testo avanzato della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Tutti gli oggetti Characters. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Indica se questa cella è impostata come casella di controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Imposta una formula di matrice dinamica e fa sì che la formula si estenda alle celle adiacenti, se possibile.

**Remarks**

l'intervallo restituito potrebbe non coincidere con quello reale in cui questa formula di matrice dinamica si espande. Se ci sono celle non vuote nell'intervallo, la formula verrà impostata solo per la cella corrente e contrassegnata come "\#SPILL!". Tuttavia, in questo tipo di situazione restituiamo comunque l'intero intervallo in cui la formula dovrebbe espandersi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | l'espressione della formula |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | opzioni per analizzare la formula. L'opzione "Parse" verrà ignorata e la formula sarà sempre analizzata immediatamente |
| calculateValue | boolean | se calcolare questa formula di matrice dinamica per quelle celle nell'intervallo espanso. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Imposta una formula di matrice dinamica e fa sì che la formula si estenda alle celle adiacenti, se possibile.

**Remarks**

l'intervallo restituito potrebbe non coincidere con quello reale in cui questa formula di matrice dinamica si espande. Se ci sono celle non vuote nell'intervallo, la formula verrà impostata solo per la cella corrente e contrassegnata come "\#SPILL!". Tuttavia, in questo tipo di situazione restituiamo comunque l'intero intervallo in cui la formula dovrebbe espandersi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | l'espressione della formula |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | opzioni per analizzare la formula. L'opzione "Parse" verrà ignorata e la formula sarà sempre analizzata immediatamente |
| valori | java.lang.Object[][] | valori (risultati calcolati) per quelle celle con la formula di matrice dinamica fornita |
| calculateRange | boolean | Se calcolare l'intervallo espanso per questa formula di matrice dinamica. Se il parametro "values" non è null e questa flag è false, l'altezza dell'intervallo espanso sarà values.Length e la larghezza sarà values[0].Length. |
| calculateValue | boolean | se calcolare questa formula di matrice dinamica per quelle celle nell'intervallo espanso quando "values" è null o l'elemento corrispondente in "values" per una cella è null. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Imposta una formula di matrice dinamica e fa sì che la formula si estenda alle celle adiacenti, se possibile.

**Remarks**

l'intervallo restituito potrebbe non coincidere con quello reale in cui questa formula di matrice dinamica si espande. Se ci sono celle non vuote nell'intervallo, la formula verrà impostata solo per la cella corrente e contrassegnata come "\#SPILL!". Tuttavia, in questo tipo di situazione restituiamo comunque l'intero intervallo in cui la formula dovrebbe espandersi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | java.lang.String | l'espressione della formula |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | opzioni per analizzare la formula. L'opzione "Parse" verrà ignorata e la formula sarà sempre analizzata immediatamente |
| valori | java.lang.Object[][] | valori (risultati calcolati) per quelle celle con la formula di matrice dinamica fornita |
| calculateRange | boolean | Se calcolare l'intervallo espanso per questa formula di matrice dinamica. Se il parametro "values" non è null e questa flag è false, l'altezza dell'intervallo espanso sarà values.Length e la larghezza sarà values[0].Length. |
| calculateValue | boolean | se calcolare questa formula di matrice dinamica per quelle celle nell'intervallo espanso quando "values" è null o l'elemento corrispondente in "values" per una cella è null. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Le opzioni per il calcolo della formula. Comunemente, per motivi di prestazioni, la proprietà [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\#getRecursive--) dovrebbe essere false. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Imposta l'immagine incorporata nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Imposta una formula della [Cell](../../com.aspose.cells/cell).

**Remarks**

Una stringa di formula inizia sempre con un segno di uguale (=). E si prega di utilizzare sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Imposta la formula e il valore della formula.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.SetFormula(string,FormulaParseOptions,object). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2019. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula. |
| isR1C1 | boolean | Se la formula è una formula R1C1. |
| isLocal | boolean | Se la formula è formattata per la locale. |
| valore | java.lang.Object | Il valore della formula. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Imposta la formula e il valore (risultato calcolato) della formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Imposta la formula e il valore (risultato calcolato) della formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |
| valore | java.lang.Object | Il valore (risultato calcolato) della formula. |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Imposta la formula e il valore (risultato calcolato) della formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula. |
| valore | java.lang.Object | Il valore (risultato calcolato) della formula. |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Ottieni la formula formattata in base alla locale della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Imposta la stringa HTML che contiene dati e alcuni formati in questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


Imposta una formula R1C1 della [Cell](../../com.aspose.cells/cell).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Imposta formule condivise a un intervallo di celle.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formula condivisa. |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Imposta una formula a un intervallo di celle.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2019. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formula condivisa. |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| isR1C1 | boolean | se la formula è una formula R1C1 |
| isLocal | boolean | se la formula è formattata secondo la locale |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Imposta formule condivise a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formula condivisa. |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Imposta formule condivise a un intervallo di celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | java.lang.String | Formula condivisa. |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |
| valori | java.lang.Object[][] | valori per quelle celle con la formula condivisa fornita |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Imposta lo stile della cella.

**Remarks**

Se le impostazioni del bordo vengono modificate, il bordo delle celle di regolazione verrà aggiornato anch'esso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Lo stile della cella. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Applica la proprietà modificata dello stile alla cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Lo stile della cella. |
| explicitFlag | boolean | True, sovrascrive solo la formattazione che è impostata esplicitamente. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Applica lo stile della cella in base ai flag.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Lo stile della cella. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Il flag di stile. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| rowIndexOfInputCell | int | indice di riga della cella di input |
| columnIndexOfInputCell | int | indice di colonna della cella di input |
| isRowInput | boolean | Indica se la cella di input è una cella di input riga (true) o una cella di input colonna (false). |
| valori | java.lang.Object[][] | valori per le celle nell'intervallo di formula della tabella |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| rowIndexOfRowInputCell | int | indice di riga della cella di input riga |
| columnIndexOfRowInputCell | int | indice di colonna della cella di input riga |
| rowIndexOfColumnInputCell | int | indice di riga della cella di input colonna |
| columnIndexOfColumnInputCell | int | indice di colonna della cella di input colonna |
| valori | java.lang.Object[][] | valori per le celle nell'intervallo di formula della tabella |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| inputCell | java.lang.String | la cella di input |
| isRowInput | boolean | Indica se la cella di input è una cella di input riga (true) o una cella di input colonna (false). |
| valori | java.lang.Object[][] | valori per le celle nell'intervallo di formula della tabella |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | int | Numero di righe da popolare nella formula. |
| columnNumber | int | Numero di colonne da popolare nella formula. |
| rowInputCell | java.lang.String | la cella di input della riga |
| columnInputCell | java.lang.String | la cella di input della colonna |
| valori | java.lang.Object[][] | valori per le celle nell'intervallo di formula della tabella |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Imposta il valore contenuto in questa cella.

**Remarks**

Tipo possibile:

null,

Boolean,

DateTime,

Double,

Integer

String.

Per un valore int, può essere restituito come un oggetto Integer o un oggetto Double. E non c'è alcuna garanzia che il valore restituito rimanga sempre dello stesso tipo di oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


Converti la [Cell](../../com.aspose.cells/cell) in dati struct JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta l'oggetto Cell corrente.

**Returns:**
java.lang.String -
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

