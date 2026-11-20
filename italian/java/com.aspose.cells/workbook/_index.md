---
title: "Workbook"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un oggetto radice per creare un foglio di calcolo Excel."
type: docs
url: /it/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Rappresenta un oggetto radice per creare un foglio di calcolo Excel.

**Remarks**

La classe Workbook indica un foglio di calcolo Excel. Ogni foglio di calcolo può contenere più fogli di lavoro. La funzionalità di base della classe è aprire e salvare file Excel nativi. La classe ha alcune funzionalità avanzate, come copiare dati da altri Workbook, combinare due Workbook, convertire Excel in PDF, renderizzare Excel in immagine e proteggere il foglio di calcolo Excel.

**Example**

Il seguente esempio carica un Workbook da un file Excel denominato designer.xls e rende invisibili le barre di scorrimento orizzontali e verticali. Quindi sostituisce due valori stringa con un valore intero e un valore stringa rispettivamente all'interno del foglio di calcolo e infine salva il workbook come file Excel xlsx.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Workbook()](#Workbook--) | Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(int fileFormatType)](#Workbook-int-) | Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Inizializza una nuova istanza vuota della classe [Workbook](../../com.aspose.cells/workbook) con opzioni |
| [Workbook(String file)](#Workbook-java.lang.String-) | Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre un file. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre uno stream. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre un file. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre lo stream. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Accetta tutte le modifiche tracciate nella cartella di lavoro. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive). |
| [calculateFormula()](#calculateFormula--) | Calcola il risultato delle formule. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Calcola il risultato delle formule. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Calcolo delle formule in questa cartella di lavoro. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Modifica la tavolozza per il foglio di calcolo nell'indice specificato. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Chiude la sessione che utilizza cache per accedere ai dati. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Combina un altro oggetto Workbook. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Copia i dati da un oggetto Workbook di origine. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Copia un altro oggetto Workbook. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Copia il tema da un'altra cartella di lavoro. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Crea uno stile predefinito del tipo specificato. |
| [createCellsColor()](#createCellsColor--) | Crea un oggetto [CellsColor](../../com.aspose.cells/cellscolor). |
| [createStyle()](#createStyle--) | Crea un nuovo stile. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Crea un nuovo stile. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Personalizza il tema. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Esporta i dati XML collegati dalla mappa XML specificata. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Esporta i dati XML collegati dalla mappa XML specificata. |
| [getAbsolutePath()](#getAbsolutePath--) | Ottiene il percorso assoluto del file. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento integrate del foglio di calcolo. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Ottiene la fabbrica per creare ICellsDataTable da oggetti personalizzati. |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Restituisce i colori nella tavolozza per il foglio di calcolo. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Ottiene l'elenco degli oggetti [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) nella cartella di lavoro. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Ottiene il numero degli stili nel pool di stili. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto). |
| [getDataConnections()](#getDataConnections--) | Ottiene la collezione [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getDataMashup()](#getDataMashup--) | Ottiene i dati mashup. |
| [getDataModel()](#getDataModel--) | Ottiene il modello di dati nella cartella di lavoro. |
| [getDataSorter()](#getDataSorter--) | Ottiene un oggetto DataSorter per ordinare i dati. |
| [getDefaultStyle()](#getDefaultStyle--) | Ottiene l'oggetto [Style](../../com.aspose.cells/style) predefinito della cartella di lavoro. |
| [getDigitalSignature()](#getDigitalSignature--) | Ottiene la firma digitale dal file. |
| [getFileFormat()](#getFileFormat--) | Ottiene il formato del file. |
| [getFileName()](#getFileName--) | Ottiene il nome file corrente. |
| [getFonts()](#getFonts--) | Ottiene tutti i caratteri nel pool di stili. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Ottiene il monitor di interruzione. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Trova il colore più corrispondente nella palette corrente. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Ottiene lo stile denominato nel pool di stili. |
| [getRibbonXml()](#getRibbonXml--) | Ottiene il file XML che definisce l'interfaccia Ribbon. |
| [getSettings()](#getSettings--) | Rappresenta le impostazioni della cartella di lavoro. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Ottiene lo stile nel pool di stili. |
| [getTheme()](#getTheme--) | Ottiene il nome del tema. |
| [getThemeColor(int type)](#getThemeColor-int-) | Ottiene il colore del tema. |
| [getVbaProject()](#getVbaProject--) | Ottiene il [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) in un foglio di calcolo. |
| [getWorksheets()](#getWorksheets--) | Ottiene la collezione [WorksheetCollection](../../com.aspose.cells/worksheetcollection) nel foglio di calcolo. |
| [hasCustomFunction()](#hasCustomFunction--) | Rileva se è presente una funzione personalizzata utilizzata in questa cartella di lavoro, ad esempio nella formula di una cella, nei nomi definiti... |
| [hasExernalLinks()](#hasExernalLinks--) | Indica se questa cartella di lavoro contiene collegamenti esterni ad altre fonti di dati. |
| [hasMacro()](#hasMacro--) | Indica se questo foglio di calcolo contiene macro/VBA. |
| [hasRevisions()](#hasRevisions--) | Ottiene se la cartella di lavoro ha modifiche tracciate. |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Importa/Aggiorna un file dati XML nella cartella di lavoro. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Importa/Aggiorna un file dati XML nella cartella di lavoro. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Verifica se un colore è nella palette per il foglio di calcolo. |
| [isDigitallySigned()](#isDigitallySigned--) | Indica se questo foglio di calcolo è firmato digitalmente. |
| [isLicensed()](#isLicensed--) | Indica se la licenza è impostata. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Indica se la struttura o la finestra è protetta con password. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Unisce gli stili denominati dall'altro file Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Analizza tutte le formule che non sono state analizzate quando sono state caricate dal file modello o impostate in una cella. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Protegge una cartella di lavoro. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Protegge una cartella di lavoro condivisa. |
| [refreshAll()](#refreshAll--) | Aggiorna le forme collegate, tutte le tabelle pivot e i grafici con la fonte pivot. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Aggiorna le formule di array dinamici(espandono in un nuovo intervallo di celle adiacenti in base ai dati attuali). Altre formule nella cartella di lavoro non saranno calcolate ricorsivamente anche se sono state utilizzate dalle formule di array dinamici. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Aggiorna le formule di array dinamici(espandono in un nuovo intervallo di celle adiacenti in base ai dati attuali). |
| [removeDigitalSignature()](#removeDigitalSignature--) | Rimuove la firma digitale da questo foglio di calcolo. |
| [removeExternalLinks()](#removeExternalLinks--) | Rimuove tutti i collegamenti esterni nella cartella di lavoro. |
| [removeMacro()](#removeMacro--) | Rimuove VBA/macro da questo foglio di calcolo. |
| [removePersonalInformation()](#removePersonalInformation--) | Rimuove le informazioni personali. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Rimuove tutti gli stili inutilizzati. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Sostituisce i valori delle celle con nuovi dati. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Sostituisce i valori delle celle con nuovi dati. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Sostituisce il valore di una cella con un nuovo double. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Sostituisce i valori delle celle con un array di double. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Sostituisce il valore di una cella con un nuovo intero. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Sostituisce i valori delle celle con un array di interi. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Sostituisce il valore di una cella con una nuova stringa. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Sostituisce il valore di una cella con una nuova stringa. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Sostituisce il valore di una cella con un nuovo array di stringhe. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Salva la cartella di lavoro nello stream. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Salva la cartella di lavoro nello stream. |
| [save(String fileName)](#save-java.lang.String-) | Salva la cartella di lavoro sul disco. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Salva la cartella di lavoro sul disco. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Salva la cartella di lavoro sul disco. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Imposta il percorso assoluto del file. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Imposta l'oggetto [Style](../../com.aspose.cells/style) predefinito della cartella di lavoro. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Imposta la firma digitale su un file di foglio di calcolo (Excel2007 e versioni successive). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Imposta le opzioni di crittografia. |
| [setFileFormat(int value)](#setFileFormat-int-) | Imposta il formato del file. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Imposta il nome del file corrente. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Imposta il monitor di interruzione. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Imposta il file XML che definisce l'interfaccia Ribbon. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Imposta il colore del tema |
| [startAccessCache(int opts)](#startAccessCache-int-) | Avvia la sessione che utilizza le cache per accedere ai dati. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Rimuove la protezione da una cartella di lavoro. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Rimuove la protezione da una cartella di lavoro condivisa. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Aggiorna la definizione delle funzioni personalizzate. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Se questa cartella di lavoro contiene collegamenti esterni ad altre fonti di dati, Aspose.Cells cercherà di recuperare i dati più recenti dalle fonti fornite. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Il tipo di formato file predefinito è Xlsx. Se desideri creare altri tipi di file, utilizza Workbook(FileFormatType).

**Example**

Il codice seguente mostra come utilizzare il costruttore Workbook per creare e inizializzare una nuova istanza della classe.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Il tipo di formato file predefinito è Excel97To2003.

**Example**

Il codice seguente mostra come utilizzare il costruttore Workbook per creare e inizializzare una nuova istanza della classe con diversi tipi di formato file.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). Il nuovo formato file. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Inizializza una nuova istanza vuota della classe [Workbook](../../com.aspose.cells/workbook) con opzioni

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Le opzioni. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.lang.String | Il nome del file. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.lang.String | Il nome del file. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Le opzioni di caricamento |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [Workbook](../../com.aspose.cells/workbook) e apre lo stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Le opzioni di caricamento |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Accetta tutte le modifiche tracciate nella cartella di lavoro.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive).

**Remarks**

Supporta solo l'aggiunta della firma digitale Xmldsig a un file di foglio di calcolo OOXML

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcola il risultato delle formule.

**Remarks**

Per tutte le formule supportate, consulta l'elenco all'indirizzo https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Calcola il risultato delle formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ignoreError | boolean | Indica se nascondere l'errore nel calcolo delle formule. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Calcolo delle formule in questa cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per il calcolo |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Modifica la tavolozza per il foglio di calcolo nell'indice specificato.

**Remarks**

La tavolozza ha 56 voci, ciascuna rappresentata da un valore RGB.

Se imposti un colore che non è nella tavolozza, non avrà effetto.

Quindi, se vuoi impostare un colore personalizzato, modifica prima la tavolozza.

Di seguito è la tavolozza di colori standard.

| Color | Rosso | Verde | Blu |
| ------- | --- | ----- | ---- |
| Nero | 0 | 0 | 0 |
| Bianco | 255 | 255 | 255 |
| Rosso | 255 | 0 | 0 |
| Verde lime | 0 | 255 | 0 |
| Blu | 0 | 0 | 255 |
| Giallo | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Ciano | 0 | 255 | 255 |
| Marrone | 128 | 0 | 0 |
| Verde | 0 | 128 | 0 |
| Blu marino | 0 | 0 | 128 |
| Oliva | 128 | 128 | 0 |
| Viola | 128 | 0 | 128 |
| Verde acqua | 0 | 128 | 128 |
| Argento | 192 | 192 | 192 |
| Grigio | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Colore22 | 255 | 128 | 128 |
| Colore23 | 0 | 102 | 204 |
| Colore24 | 204 | 204 | 255 |
| Colore25 | 0 | 0 | 128 |
| Colore26 | 255 | 0 | 255 |
| Colore27 | 255 | 255 | 0 |
| Colore28 | 0 | 255 | 255 |
| Colore29 | 128 | 0 | 128 |
| Colore30 | 128 | 0 | 0 |
| Colore31 | 0 | 128 | 128 |
| Colore32 | 0 | 0 | 255 |
| Colore33 | 0 | 204 | 255 |
| Colore34 | 204 | 255 | 255 |
| Colore35 | 204 | 255 | 204 |
| Colore36 | 255 | 255 | 153 |
| Colore37 | 153 | 204 | 255 |
| Colore38 | 255 | 153 | 204 |
| Colore39 | 204 | 153 | 255 |
| Colore40 | 255 | 204 | 153 |
| Colore41 | 51 | 102 | 255 |
| Colore42 | 51 | 204 | 204 |
| Colore43 | 153 | 204 | 0 |
| Colore44 | 255 | 204 | 0 |
| Colore45 | 255 | 153 | 0 |
| Colore46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Struttura del colore. |
| indice | int | Indice della palette, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Chiude la sessione che utilizza cache per accedere ai dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opzioni di accesso ai dati |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Combina un altro oggetto Workbook.

**Remarks**

Unisci Excel, ODS, CSV e altri file in un unico file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Un altro oggetto Workbook. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Copia i dati da un oggetto Workbook di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Oggetto Workbook di origine. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Copia un altro oggetto Workbook.

**Remarks**

È molto semplice clonare un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Oggetto Workbook di origine. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Le opzioni per copiare un altro workbook. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Copia il tema da un'altra cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Workbook di origine. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Crea uno stile predefinito del tipo specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). Lo stile predefinito. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Crea un oggetto [CellsColor](../../com.aspose.cells/cellscolor).

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Crea un nuovo stile.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Crea un nuovo stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Indica se clona lo stile predefinito |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Personalizza il tema.

**Remarks**

La lunghezza dei colori dovrebbe essere 12.

| Indice dell'array | Tipo di tema |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Collegamento ipertestuale |
| 11 | Collegamento ipertestuale visitato |

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| themeName | java.lang.String | Il nome del tema |
| colors | [Color\[\]](../../com.aspose.cells/color) | I colori del tema |

### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Esporta i dati XML collegati dalla mappa XML specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mapName | java.lang.String | nome della mappa XML da esportare |
| stream | java.io.OutputStream | lo stream di esportazione |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Esporta i dati XML collegati dalla mappa XML specificata.

**Example**

Il codice seguente ha esportato i dati collegati dalla prima XmlMap.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mapName | java.lang.String | nome della mappa XML da esportare |
| percorso | java.lang.String | il percorso di esportazione |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Ottiene il percorso assoluto del file.

**Remarks**

Utilizzato solo per collegamenti esterni.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento integrate del foglio di calcolo.

**Remarks**

Non è possibile aggiungere una nuova proprietà all'elenco delle proprietà documento integrate. È possibile solo ottenere una proprietà integrata e modificarne il valore. Di seguito è l'elenco dei nomi delle proprietà integrate:

Title

Oggetto

Autore

Parole chiave

Commenti

Modello

Ultimo autore

Numero di revisione

Nome dell'applicazione

Data ultima stampa

Data di creazione

Ora ultimo salvataggio

Tempo totale di modifica

Numero di pagine

Numero di parole

Numero di caratteri

Sicurezza

Categoria

Formato

Responsabile

Azienda

Numero di byte

Numero di righe

Numero di paragrafi

Numero di diapositive

Numero di note

Numero di diapositive nascoste

Numero di clip multimediali

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Ottiene la fabbrica per creare ICellsDataTable da oggetti personalizzati.

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Restituisce i colori nella tavolozza per il foglio di calcolo.

**Remarks**

La tavolozza ha 56 voci, ciascuna rappresentata da un valore RGB.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Ottiene l'elenco degli oggetti [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) nella cartella di lavoro.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Ottiene il numero degli stili nel pool di stili.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Ottiene la collezione [ExternalConnection](../../com.aspose.cells/externalconnection).

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Ottiene i dati mashup.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Ottiene il modello di dati nella cartella di lavoro.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Ottiene un oggetto DataSorter per ordinare i dati.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Ottiene l'oggetto [Style](../../com.aspose.cells/style) predefinito della cartella di lavoro.

**Remarks**

La proprietà DefaultStyle è utile per implementare uno Stile per l'intero Workbook.

**Example**

Il codice seguente crea e istanzia un nuovo Workbook e imposta uno Stile predefinito [Stile](../../com.aspose.cells/style) su di esso.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Ottiene la firma digitale dal file.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Ottiene il formato del file.

Vedi [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Ottiene il nome file corrente.

**Remarks**

Se il file è aperto tramite stream e ci sono alcuni riferimenti a formule esterne, impostare il nome del file.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Ottiene tutti i caratteri nel pool di stili.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Ottiene il monitor di interruzione.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Trova il colore più corrispondente nella palette corrente.

**Remarks**

Ci sono solo 56 colori nella tavolozza dei colori in Excel 97-2003. Se il colore non è nella tavolozza, verrà impostato il colore più simile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Colore grezzo. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Ottiene lo stile denominato nel pool di stili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | nome dello stile |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Ottiene il file XML che definisce l'interfaccia Ribbon.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Rappresenta le impostazioni della cartella di lavoro.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Ottiene lo stile nel pool di stili. Tutti gli stili nel workbook saranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento.

**Remarks**

Se lo stile restituito viene modificato, lo stile di tutte le celle (che fanno riferimento a questo stile) verrà modificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Ottiene il nome del tema.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Ottiene il colore del tema.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Il tipo di colore del tema. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Ottiene il [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) in un foglio di calcolo.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Ottiene la collezione [WorksheetCollection](../../com.aspose.cells/worksheetcollection) nel foglio di calcolo.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Rileva se è presente una funzione personalizzata utilizzata in questa cartella di lavoro, ad esempio nella formula di una cella, nei nomi definiti...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Indica se questa cartella di lavoro contiene collegamenti esterni ad altre fonti di dati.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare ExternalLinkCollection.Count per verificare se ci sono collegamenti esterni in questo workbook. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean - Indica se questo workbook contiene collegamenti esterni ad altre fonti di dati.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Indica se questo foglio di calcolo contiene macro/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Ottiene se la cartella di lavoro ha modifiche tracciate.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Importa/Aggiorna un file dati XML nella cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | lo stream del file xml. |
| sheetName | java.lang.String | il nome del foglio di destinazione. |
| riga | int | la riga di destinazione. |
| col | int | la colonna di destinazione. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Importa/Aggiorna un file dati XML nella cartella di lavoro.

**Example**

Il codice seguente importa dati xml nel foglio di lavoro 'Sheet 1' nella cella A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| url | java.lang.String | l'url/percorso del file xml. |
| sheetName | java.lang.String | il nome del foglio di destinazione. |
| riga | int | la riga di destinazione |
| col | int | la colonna di destinazione |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Verifica se un colore è nella palette per il foglio di calcolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Struttura del colore. |

**Returns:**
boolean - Restituisce true se questo colore è nella palette. Altrimenti, restituisce false
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Indica se questo foglio di calcolo è firmato digitalmente.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Indica se la licenza è impostata.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Indica se la struttura o la finestra è protetta con password.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Unisce gli stili denominati dall'altro file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | L'altro file |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Analizza tutte le formule che non sono state analizzate quando sono state caricate dal file modello o impostate in una cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ignoreError | boolean | Indica se ignorare l'errore per una formula non valida. Per una formula non valida, se si ignora l'errore la formula verrà ignorata e il processo continuerà ad analizzare le altre formule, altrimenti verrà sollevata un'eccezione. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Protegge una cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo di protezione. |
| password | java.lang.String | Password per proteggere la cartella di lavoro. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Protegge una cartella di lavoro condivisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | Password per proteggere la cartella di lavoro. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Aggiorna le forme collegate, tutte le tabelle pivot e i grafici con la fonte pivot.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Aggiorna le formule di array dinamici(espandono in un nuovo intervallo di celle adiacenti in base ai dati attuali). Altre formule nella cartella di lavoro non saranno calcolate ricorsivamente anche se sono state utilizzate dalle formule di array dinamici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calcolare | boolean | Indica se calcolare e aggiornare i valori delle celle per quelle formule di array dinamici |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Aggiorna le formule di array dinamici(espandono in un nuovo intervallo di celle adiacenti in base ai dati attuali).

**Remarks**

Per motivi di prestazioni, non aggiorniamo automaticamente tutte le formule di array dinamici quando la formula stessa o i dati a cui fa riferimento cambiano. Pertanto l'utente deve chiamare questo metodo manualmente dopo le operazioni che possono influenzare le formule di array dinamici, come l'importazione/impostazione dei valori delle celle, l'inserimento/eliminazione di righe/colonne/intervalli, ...etc.

Per la maggior parte delle formule con funzioni, il calcolo dell'intervallo di spill richiede anche il calcolo della formula, quindi in generale è preferibile il valore true per il flag \"calculate\". Se la formula è semplice, ad esempio un riferimento a un intervallo o un array (per esempio \"=C1:E5\", \"=\\{1,2;3,4\\}\", ...), una funzione semplice su un intervallo o un array (per esempio \"=ABS(C1:E5)\", \"=1+\\{1,2;3,4\\}\", ...), e tutte le formule verranno calcolate in seguito (ad esempio tramite [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-)), allora utilizzare il valore false per il flag \"calculate\" può evitare il calcolo duplicato a beneficio delle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calcolare | boolean | Indica se calcolare e aggiornare i valori delle celle per quelle formule di array dinamici |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Le opzioni per il calcolo delle formule |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Rimuove la firma digitale da questo foglio di calcolo.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Rimuove tutti i collegamenti esterni nella cartella di lavoro.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo ExternalLinkCollection.Clear(). Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Rimuove VBA/macro da questo foglio di calcolo.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Rimuove le informazioni personali.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Rimuove tutti gli stili inutilizzati.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Sostituisce i valori delle celle con nuovi dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| boolValue | boolean | Il valore booleano da sostituire. |
| newValue | java.lang.Object | Nuovo valore. Può essere stringa, intero, double o valore DateTime. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Sostituisce i valori delle celle con nuovi dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intValue | int | Il valore intero da sostituire. |
| newValue | java.lang.Object | Nuovo valore. Può essere stringa, intero, double o valore DateTime. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Sostituisce il valore di una cella con un nuovo double.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValue | double | Valore double da sostituire |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Sostituisce i valori delle celle con un array di double.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValues | double[] | Array di double da sostituire |
| isVertical | boolean | True - Verticale, False - Orizzontale |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Sostituisce il valore di una cella con un nuovo intero.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValue | int | Valore intero da sostituire |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Sostituisce i valori delle celle con un array di interi.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValues | int[] | Array di interi da sostituire |
| isVertical | boolean | True - Verticale, False - Orizzontale |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Sostituisce il valore di una cella con una nuova stringa.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValue | java.lang.String | Valore stringa da sostituire |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Sostituisce il valore di una cella con una nuova stringa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValue | java.lang.String | Valore stringa da sostituire |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Le opzioni di sostituzione |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Sostituisce il valore di una cella con un nuovo array di stringhe.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | java.lang.String | Segnaposto cella |
| newValues | java.lang.String[] | Array di stringhe da sostituire |
| isVertical | boolean | True - Verticale, False - Orizzontale |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Salva la cartella di lavoro nello stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso del file. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Le opzioni di salvataggio. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Salva la cartella di lavoro nello stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso del file. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Il tipo di formato file di salvataggio. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Salva la cartella di lavoro sul disco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Salva la cartella di lavoro sul disco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Le opzioni di salvataggio. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Salva la cartella di lavoro sul disco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Il tipo di formato di salvataggio. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Imposta il percorso assoluto del file.

**Remarks**

Utilizzato solo per collegamenti esterni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Imposta l'oggetto [Style](../../com.aspose.cells/style) predefinito della cartella di lavoro.

**Remarks**

La proprietà DefaultStyle è utile per implementare uno Stile per l'intero Workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Imposta la firma digitale su un file di foglio di calcolo (Excel2007 e versioni successive).

**Remarks**

Supporta solo l'aggiunta di Xmldsig Digital Signature

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Imposta le opzioni di crittografia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). Il tipo di crittografia. |
| keyLength | int | La lunghezza della chiave. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Imposta il formato del file.

Vedi [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Imposta il nome del file corrente.

**Remarks**

Se il file è aperto tramite stream e ci sono alcuni riferimenti a formule esterne, impostare il nome del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Imposta il monitor di interruzione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Imposta il file XML che definisce l'interfaccia Ribbon.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Imposta il colore del tema

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Il tipo di colore del tema. |
| color | [Color](../../com.aspose.cells/color) | il colore del tema |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Avvia la sessione che utilizza le cache per accedere ai dati.

**Remarks**

Se la cache dell'accesso ai dati specificati richiede che alcuni modelli di dati nel foglio di lavoro siano "read-only", allora i modelli di dati corrispondenti in ogni foglio di lavoro di questa cartella di lavoro saranno considerati "read-only" e l'utente non dovrebbe modificarne alcuno.

Dopo aver terminato l'accesso ai dati, [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) dovrebbe essere invocato con le stesse opzioni per cancellare tutte le cache e ripristinare la modalità di accesso normale.



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opzioni di accesso ai dati |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Rimuove la protezione da una cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | Password per rimuovere la protezione della cartella di lavoro. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Rimuove la protezione da una cartella di lavoro condivisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | Password per rimuovere la protezione della cartella di lavoro. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Aggiorna la definizione delle funzioni personalizzate.

**Remarks**

Questo metodo può essere utilizzato per alcuni scenari speciali. Ad esempio, se l'utente ha bisogno che alcuni parametri di funzioni personalizzate vengano calcolati in modalità array, allora l'utente può fornire la propria definizione con l'implementazione di [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) per tali funzioni. Dopo che i dati delle formule sono stati aggiornati, i parametri specificati verranno calcolati automaticamente in modalità array durante il calcolo delle funzioni personalizzate corrispondenti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Definizione speciale di funzioni personalizzate per i requisiti speciali dell'utente. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Se questa cartella di lavoro contiene collegamenti esterni ad altre fonti di dati, Aspose.Cells cercherà di recuperare i dati più recenti dalle fonti fornite.

**Remarks**

Se il collegamento esterno corrispondente non può essere trovato per una cartella di lavoro, allora questa cartella di lavoro verrà ignorata. Pertanto, quando impostate in seguito una formula con un nuovo collegamento esterno che intendete collegare alla cartella di lavoro ignorata, il collegamento non potrà essere effettuato finché non richiamate nuovamente questo metodo con quelle cartelle di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Cartelle di lavoro che saranno utilizzate per aggiornare i dati dei collegamenti esterni referenziati da questa cartella di lavoro. L'abbinamento di tali cartelle di lavoro con i collegamenti esterni è determinato da [getFileName()](../../com.aspose.cells/workbook\#getFileName--) e [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Pertanto, assicuratevi che [getFileName()](../../com.aspose.cells/workbook\#getFileName--) sia stato specificato con il valore corretto per ogni cartella di lavoro affinché possa essere collegata al collegamento esterno corrispondente. |

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

