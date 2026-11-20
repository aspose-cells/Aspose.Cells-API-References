---
title: "CellsHelper"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Fornisce funzioni di supporto."
type: docs
url: /it/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Fornisce funzioni di supporto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Aggiungi la funzione add-in. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Ottiene gli indici di riga e colonna della cella in base al suo nome. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Ottiene il nome della colonna in base all'indice della colonna. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Ottiene l'indice della colonna in base al nome della colonna. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Converte la formula A1 della cella nella formula r1c1. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Converte la formula r1c1 della cella nella formula A1. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Verifica il nome del foglio fornito e crea uno valido se necessario. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Verifica il nome del foglio fornito e crea uno valido se necessario. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Ottiene il percorso di avvio alternativo, a cui fanno riferimento alcune formule esterne. |
| [getCacheFolder()](#getCacheFolder--) | Ottiene la cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Ottiene la fabbrica per creare istanze con implementazione speciale. |
| [getDPI()](#getDPI--) | Ottiene i DPI della macchina. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Converti il valore double in valore data/ora. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Converti la data/ora in valore double. |
| [getLibraryPath()](#getLibraryPath--) | Ottiene il percorso della libreria a cui fanno riferimento alcune formule esterne. |
| [getSignificantDigits()](#getSignificantDigits--) | Ottiene il numero di cifre significative. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Ottiene il tipo predefinito di cifre significative per l'emissione di valori numerici. |
| [getStartupPath()](#getStartupPath--) | Ottiene il percorso di avvio a cui fanno riferimento alcune formule esterne. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Ottieni la larghezza del testo in unità di punti. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Ottiene tutti i colori usati nella cartella di lavoro. |
| [getVersion()](#getVersion--) | Ottieni la versione di rilascio. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Unisce alcuni file xls di grandi dimensioni in un file xls. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Indica se il nome del foglio deve essere racchiuso tra virgolette singole. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Ottiene il nome della riga in base all'indice della riga. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Ottiene l'indice della riga in base al nome della riga. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Imposta il percorso di avvio alternativo, a cui fanno riferimento alcune formule esterne. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Imposta la cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Imposta la fabbrica per creare istanze con implementazione speciale. |
| [setDPI(double value)](#setDPI-double-) | Ottiene i DPI della macchina. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Imposta il percorso della libreria a cui si riferiscono alcuni riferimenti di formula esterni. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Imposta il numero di cifre significative. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Imposta il tipo predefinito di cifre significative per l'emissione di valori numerici. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Imposta il percorso di avvio, a cui si riferiscono alcuni riferimenti di formula esterni. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Aggiungi la funzione add-in.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare i metodi WorksheetCollection.RegisterAddInFunction(). Questo metodo sarà rimosso 12 mesi dopo, a partire da gennaio 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| funzione | java.lang.String | Il nome della funzione. |
| minCountOfParameters | int | Numero minimo di parametri richiesti da questa funzione |
| maxCountOfParameters | int | Numero massimo di parametri consentiti da questa funzione. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). Il tipo di parametri previsto della funzione |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). Il tipo di valore della funzione. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Ottiene il nome della cella in base ai suoi indici di riga e colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |

**Returns:**
java.lang.String - Nome della cella.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Ottiene gli indici di riga e colonna della cella in base al suo nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella |

**Returns:**
int[] - [0] è l'indice di riga e [1] è l'indice di colonna.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Ottiene il nome della colonna in base all'indice della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

**Returns:**
java.lang.String - Nome della colonna.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Ottiene l'indice della colonna in base al nome della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnName | java.lang.String | Nome della colonna. |

**Returns:**
int - Indice di colonna.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Converte la formula A1 della cella nella formula r1c1.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.ConvertFormulaReferenceStyle(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula A1. |
| riga | int | L'indice di riga della cella. |
| colonna | int | L'indice di colonna della cella. |

**Returns:**
java.lang.String - La formula R1C1.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Converte la formula r1c1 della cella nella formula A1.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.ConvertFormulaReferenceStyle(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| r1c1Formula | java.lang.String | La formula r1c1. |
| riga | int | L'indice di riga della cella. |
| colonna | int | L'indice di colonna della cella. |

**Returns:**
java.lang.String - La formula A1.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con ' ', quindi verrà restituito il valore della stringa ricostruita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nameProposal | java.lang.String | nome del foglio da utilizzare |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con il carattere fornito, quindi verrà restituito il valore della stringa ricostruita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nameProposal | java.lang.String | nome del foglio da utilizzare |
| replaceChar | char | carattere che verrà usato per sostituire i caratteri non validi nel nome del foglio fornito |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Ottiene il percorso di avvio alternativo, a cui fanno riferimento alcune formule esterne.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Ottiene la cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

I file di cache sono generalmente usati per alcune funzionalità per considerazioni di prestazioni della memoria, come il salvataggio di grandi set di dati in file xls o l'uso della modalità memoria con cache su file per il modello delle celle.

**Returns:**
java.lang.String - Cartella per i file di cache specificata. Se non è stata specificata, verrà restituito null e verrà usato il percorso temporaneo del sistema quando necessario.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Ottiene la fabbrica per creare istanze con implementazione speciale.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Ottiene i DPI della macchina.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Converti il valore double in valore data/ora.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleValue | double | Il valore double. |
| date1904 | boolean | Sistema data 1904. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Converti la data/ora in valore double.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | La data e ora. |
| date1904 | boolean | Sistema data 1904. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Ottiene il percorso della libreria a cui fanno riferimento alcune formule esterne.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Ottiene il numero di cifre significative. Il valore predefinito è 17.

**Remarks**

Può essere solo 15 o 17 ora. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Ottiene il tipo predefinito di cifre significative per l'output dei valori numerici. Il valore predefinito è [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Vedi [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Ottiene il percorso di avvio a cui fanno riferimento alcune formule esterne.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Ottieni la larghezza del testo in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo. |
| font | [Font](../../com.aspose.cells/font) | Il carattere del testo. |
| scalatura | double | Il ridimensionamento del testo. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Ottiene tutti i colori usati nella cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | L'oggetto workbook. |

**Returns:**
com.aspose.cells.Color[] - I colori utilizzati.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Ottieni la versione di rilascio.

**Returns:**
java.lang.String - La versione di rilascio.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Unisce alcuni file xls di grandi dimensioni in un file xls.

**Remarks**

Questo metodo supporta solo l'unione di dati, stili e formule nel nuovo file. Il file nella cache viene utilizzato per memorizzare alcuni dati temporanei.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.lang.String[] | I file. |
| cachedFile | java.lang.String | Il file nella cache. |
| destFile | java.lang.String | Il file di destinazione. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Indica se il nome del foglio deve essere racchiuso tra virgolette singole.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Il nome del foglio |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Ottiene il nome della riga in base all'indice della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |

**Returns:**
java.lang.String - Nome della riga.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Ottiene l'indice della riga in base al nome della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowName | java.lang.String | Nome della riga. |

**Returns:**
int - Indice della riga.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Imposta il percorso di avvio alternativo, a cui fanno riferimento alcune formule esterne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Imposta la cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

I file di cache sono generalmente usati per alcune funzionalità per considerazioni di prestazioni della memoria, come il salvataggio di grandi set di dati in file xls o l'uso della modalità memoria con cache su file per il modello delle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cache | java.lang.String | Cartella per i file temporanei che possono essere usati come cache dei dati. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Imposta questa proprietà su True quando si esegue su una piattaforma cloud, come: Azure, AWSLambda, ecc,

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Imposta la fabbrica per creare istanze con implementazione speciale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Ottiene i DPI della macchina.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Imposta il percorso della libreria a cui si riferiscono alcuni riferimenti di formula esterni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Imposta il numero di cifre significative. Il valore predefinito è 17.

**Remarks**

Può essere solo 15 o 17 ora. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Imposta il tipo predefinito di cifre significative per la visualizzazione dei valori numerici. Il valore predefinito è [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Vedi [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Imposta il percorso di avvio, a cui si riferiscono alcuni riferimenti di formula esterni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

