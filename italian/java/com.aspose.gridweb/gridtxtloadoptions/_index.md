---
title: "GridTxtLoadOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per il caricamento di file di testo."
type: docs
url: /it/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Rappresenta le opzioni per il caricamento di file di testo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Crea le opzioni per il caricamento di file di testo. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [getCheckDataValid()](#getCheckDataValid--) | Verifica se i dati sono validi nel file modello. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Restituisce un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. |
| [getConvertNumericData()](#getConvertNumericData--) | Restituisce un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [getEncoding()](#getEncoding--) | Ottiene la codifica predefinita. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Indica se estende i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [getKeepPrecision()](#getKeepPrecision--) | Indica se non analizzare un valore stringa quando la lunghezza è 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. |
| [getOnlyAuto()](#getOnlyAuto--) | Indica se adattare solo le righe la cui altezza non è personalizzata. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indica se analizzare la formula durante la lettura del file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. |
| [getPassword()](#getPassword--) | Ottiene la password della cartella di lavoro. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [getSeparator()](#getSeparator--) | Ottiene il separatore di caratteri del file di testo. |
| [getSeparatorString()](#getSeparatorString--) | Ottiene un valore stringa come separatore. |
| [getTextQualifier()](#getTextQualifier--) | Specifica il qualificatore di testo per i valori delle celle. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Indica se i delimitatori consecutivi devono essere trattati come uno solo. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. |
| [hasFormula()](#hasFormula--) | Indica se il testo è una formula se inizia con "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Indica se esiste un qualificatore di testo per il valore della cella. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True indica che il file contiene diverse codifiche. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Verifica se i dati sono validi nel file modello. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Imposta un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Imposta la codifica predefinita. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Indica se estende i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indica se il testo è una formula se inizia con "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Indica se esiste un qualificatore di testo per il valore della cella. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indica se non analizzare un valore stringa quando la lunghezza è 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True indica che il file contiene diverse codifiche. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indica se adattare solo le righe la cui altezza non è personalizzata. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indica se analizzare la formula durante la lettura del file. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Imposta la password del workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [setSeparator(char value)](#setSeparator-char-) | Imposta il separatore di caratteri del file di testo. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Imposta un valore stringa come separatore. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Specifica il qualificatore di testo per i valori delle celle. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Indica se i delimitatori consecutivi devono essere trattati come uno solo. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Crea le opzioni per il caricamento di file di testo.

**Remarks**

Il tipo di file di caricamento predefinito è CSV.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indica se filtrare automaticamente i dati durante il caricamento dei file.

**Remarks**

A volte, sebbene l'autofiltro sia impostato, le righe corrispondenti non sono nascoste nel file. Ora funziona solo per i file SpreadSheetML.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Verifica se i dati sono validi nel file modello.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è invalido per il formato file Excel, non dovresti salvare il workbook in formato Excel successivamente. Altrimenti potrebbero verificarsi errori inattesi nel file Excel generato.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Restituisce un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Restituisce un valore che indica se la stringa nel file di testo viene convertita in dati numerici.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ottiene la codifica predefinita. Si applica solo ai file csv.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Se questa proprietà è true, i dati aggiuntivi saranno estesi al foglio successivo dietro quello corrente (se il foglio corrente è l'ultimo, un nuovo foglio sarà aggiunto alla cartella di lavoro corrente). Se questa proprietà è false, i dati che superano il limite saranno ignorati. Il valore predefinito è false;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignora i dati che non vengono stampati se si stampa direttamente il file

**Remarks**

Solo per file xlsx.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Indica se non analizzare un valore stringa quando la lunghezza è 15.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Indica se mantenere i dati non analizzati in memoria per il Workbook quando viene caricato da un file modello. Il valore predefinito è true.

**Remarks**

Per scenari in cui l'utente deve solo leggere alcuni contenuti dal file modello e non necessita di salvare nuovamente il workbook, impostare questa proprietà su false può migliorare le prestazioni, soprattutto se usata insieme a qualche tipo di LoadFilter,

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indica se adattare solo le righe la cui altezza non è personalizzata.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indica se analizzare la formula durante la lettura del file.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm e Xlsm perché le formule nei file sono memorizzate come stringa di formula.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indica se analizzare i record cache dei pivot durante il caricamento del file. Il valore predefinito è false.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm, Xlsm e xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Ottiene la password della cartella di lavoro.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

Dopo aver caricato la cartella di lavoro dal file modello con questa opzione, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) verrà impostato allo stesso valore di questa proprietà.

**Returns:**
boolean
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Ottiene il separatore di caratteri del file di testo.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Ottiene un valore stringa come separatore.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'.

**Remarks**

Quando si imposta questa proprietà, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) diventerà true automaticamente.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Indica se i delimitatori consecutivi devono essere trattati come uno solo.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale sarà rimosso dal valore della cella corrispondente e [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) sarà impostato su true per la cella.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indica se il testo è una formula se inizia con "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


True indica che il file contiene diverse codifiche.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Indica se filtrare automaticamente i dati durante il caricamento dei file.

**Remarks**

A volte, sebbene l'autofiltro sia impostato, le righe corrispondenti non sono nascoste nel file. Ora funziona solo per i file SpreadSheetML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Verifica se i dati sono validi nel file modello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è invalido per il formato file Excel, non dovresti salvare il workbook in formato Excel successivamente. Altrimenti potrebbero verificarsi errori inattesi nel file Excel generato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Imposta un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Imposta la codifica predefinita. Si applica solo ai file csv.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Se questa proprietà è true, i dati aggiuntivi saranno estesi al foglio successivo dietro quello corrente (se il foglio corrente è l'ultimo, un nuovo foglio sarà aggiunto alla cartella di lavoro corrente). Se questa proprietà è false, i dati che superano il limite saranno ignorati. Il valore predefinito è false;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Indica se il testo è una formula se inizia con "=".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignora i dati che non vengono stampati se si stampa direttamente il file

**Remarks**

Solo per file xlsx.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Indica se non analizzare un valore stringa quando la lunghezza è 15.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Indica se mantenere i dati non analizzati in memoria per il Workbook quando viene caricato da un file modello. Il valore predefinito è true.

**Remarks**

Per scenari in cui l'utente deve solo leggere alcuni contenuti dal file modello e non necessita di salvare nuovamente il workbook, impostare questa proprietà su false può migliorare le prestazioni, soprattutto se usata insieme a qualche tipo di LoadFilter,

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True indica che il file contiene diverse codifiche.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Indica se adattare solo le righe la cui altezza non è personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Indica se analizzare la formula durante la lettura del file.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm e Xlsm perché le formule nei file sono memorizzate come stringa di formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Indica se analizzare i record cache dei pivot durante il caricamento del file. Il valore predefinito è false.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm, Xlsm e xlsb.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Imposta la password del workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

Dopo aver caricato la cartella di lavoro dal file modello con questa opzione, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) verrà impostato allo stesso valore di questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Imposta il separatore di caratteri del file di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Imposta un valore stringa come separatore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'.

**Remarks**

Quando si imposta questa proprietà, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) diventerà true automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Indica se i delimitatori consecutivi devono essere trattati come uno solo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale sarà rimosso dal valore della cella corrispondente e [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) sarà impostato su true per la cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

