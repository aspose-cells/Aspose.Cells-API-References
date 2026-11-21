---
title: "GridJsWorkbook"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar huvudindataklassen för GridJs."
type: docs
url: /sv/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Representerar huvudindataklassen för GridJs.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | Skapar en ny instans av GridJsWorkbook. |
## Fält

| Fält | Beskrivning |
| --- | --- |
| [CacheImp](#CacheImp) | Anpassad implementering för cachelagring. Om du vill lagra cache på strömbaserat sätt måste du konfigurera och implementera det. |
| [CalculateEngine](#CalculateEngine) | Anpassad implementering för beräkningsmotor, om du vill göra anpassade beräkningar måste du ange och implementera den. |
| [PICTURE_TYPE](#PICTURE-TYPE) | konstantvärde för bildens typ |
| [UpdateMonitor](#UpdateMonitor) | Hämtar/Anger uppdateringsmonitor för att spåra uppdateringsoperation |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Burns (utför) alla raderingsoperationer i arbetsboken genom att ta bort raderingsformer och deras målformer eller rensa innehållet i målcellområdet. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Kopierar bild eller form. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Hämtar felmeddelandesträngen i JSON-format. |
| [exportToJson()](#exportToJson--) | Hämtar JSON-sträng från minnesdata, standardfilnamnet i JSON är: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Hämtar JSON-sträng från minnesdata, ange utdatafilnamnet i JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Hämtar JSON-sträng från minnesdata, ange utdatafilnamnet i JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Hämtar cache‑katalogen för lagring av kalkylbladsfil. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Hämtar laddningsformatet efter filändelse |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Hämta ström av bild. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Hämtar bildens URL. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Hämtar JSON-strängen för filen från cachen med den angivna unika ID:n, sätter utdatafilnamnet i JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Hämtar bytearray-data för det inbäddade OLE-objektet. |
| [getSettings()](#getSettings--) | Representerar arbetsbokens inställningar. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Genererar ett nytt unikt ID för filcachen med hjälp av det angivna filnamnet. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Importerar Excel-filen från filström med laddningsformat. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Importerar Excel-filen från filström med laddningsformat och öppningslösenord. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importerar Excel-filen från filsökvägen. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Importerar Excel-filen från filström. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Importerar Excel-filen från filström med laddningsformat och öppningslösenord. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Importerar Excel-filen från filsökvägen. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Importerar Excel-filen från filsökväg och öppningslösenord. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Importerar Excel-filen från JSON-formatsträng. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Infogar bild i kalkylbladet från filström eller URL (antingen filström eller URL ska tillhandahållas) eller infogar form, när p.type är en av AutoShapeType. |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Generera JSON från den minnesbaserade arbetsboken och skriv den till den angivna strömmen. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Hämta JSON-strängen för filen från cachen med det angivna unika ID:t, ange utdatafilnamnet i JSON, och skriv den till strömmen. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Hämtar JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Hämta JSON-strängen för det angivna bladet i filen från cachen med det angivna unika ID:t, och skriv den till strömmen. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Tillämpar en batchuppdatering på minnesdata. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | Utför radering på en Excel-fil baserat på en array av JSON-operationer. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Sparar minnesdata till cache-filen med det angivna filnamnet och anger även öppningslösenordet, sparformatet baseras på filändelsen för filnamnet. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Sparar minnesdata till strömmen, baserat på ursprungsfilformatet. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Sparar minnesdata till filsökvägen, om filen har filändelse, sparas formatet baserat på filändelsen. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Sparar minnesdata till strömmen, sparformatet är html. |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Sparar minnesdata till filsökvägen, sparformatet är html. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Sparar minnesdata till strömmen, sparformatet är pdf. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Sparar minnesdata till filsökvägen, sparformatet är pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Sparar minnesdata till strömmen, sparformatet är xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Sparar minnesdata till filsökvägen, sparformatet är xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Ställer in cache‑katalogen för lagring av kalkylbladsfil. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Ställ in basbildens hämta‑åtgärd‑URL från kontrollern. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Ställer in InterruptMonitor för laddningsoperationen. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Ställer in InterruptMonitor för sparningsoperationen. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Representerar arbetsbokens inställningar. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Ställer in transparensen för redigeringsformer i arbetsboken. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Översätt alla strängvärden till målspråket i kalkylbladet. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Tillämpar uppdateringsoperationen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


Skapar en ny instans av GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Anpassad implementering för cachelagring. Om du vill lagra cache på strömbaserat sätt måste du konfigurera och implementera det.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Anpassad implementering för beräkningsmotor, om du vill göra anpassade beräkningar måste du ange och implementera den.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


konstantvärde för bildens typ

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Hämtar/Anger uppdateringsmonitor för att spåra uppdateringsoperation

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Burns (utför) alla raderingsoperationer i arbetsboken genom att ta bort raderingsformer och deras målformer eller rensa innehållet i målcellområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| excelFilePath | java.lang.String | Filsökvägen för Excel‑filen. |
| uid | java.lang.String | Den unika identifieraren för arbetsboken. Om null eller tom, genereras ett nytt uid baserat på filsökvägen. |

### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public void clearAllJsonCache()
```


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Kopierar bild eller form.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| p | java.lang.String | JSON‑strängen för operationen som specificerar cellplatsen, den innehåller bladnamnet, övre vänstra raden och övre vänstra kolumnen för bilden eller formen\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - JSON‑strängen för den nya kopierade bilden
### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Hämtar felmeddelandesträngen i JSON-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| msg | java.lang.String | Felmeddelandet. |

**Returns:**
java.lang.String - JSON‑strängen.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Hämtar JSON-sträng från minnesdata, standardfilnamnet i JSON är: book1.

**Returns:**
java.lang.String - JSON‑strängen.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Hämtar JSON-sträng från minnesdata, ange utdatafilnamnet i JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om det sätts till null är standardfilnamnet: book1.. |

**Returns:**
java.lang.String - JSON‑strängen.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Hämtar JSON-sträng från minnesdata, ange utdatafilnamnet i JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om det sätts till null är standardfilnamnet: book1.. |

**Returns:**
java.lang.StringBuilder - JSON‑StringBuilder.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Hämtar cache‑katalogen för lagring av kalkylbladsfil. Om detta inte är inställt använder vi den statiska egenskapen från [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) eller [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


Hämtar laddningsformatet efter filändelse

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filändelse | java.lang.String | Filändelsen börjar vanligtvis med '.'. |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Hämta ström av bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| picid | java.lang.String | Bildens id. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - Bildströmmen
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Hämtar bildens URL.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| picid | java.lang.String | Bildens id. |
| delimiter | java.lang.String | Strängavgränsaren. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Hämtar JSON-strängen för filen från cachen med den angivna unika ID:n, sätter utdatafilnamnet i JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om den sätts till null, är standardfilnamnet: book1. |

**Returns:**
java.lang.StringBuilder - JSON-sträng StringBuilder
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
```


Hämtar bytearray-data för det inbäddade OLE-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| sheetname | java.lang.String | Arbetsbladets namn. |
| oleid | int | ID för det inbäddade ole-objektet. |
| label | java.lang.String | Visningsetiketten för det inbäddade ole-objektet. |

**Returns:**
byte[] - Bytearraydata för det inbäddade ole-objektet.
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Representerar arbetsbokens inställningar.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Genererar ett nytt unikt ID för filcachen med hjälp av det angivna filnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamnet. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


Importerar Excel-filen från filström med laddningsformat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filestream | java.io.InputStream | Strömmen för Excel-filen. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat för Excel-filen. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Importerar Excel-filen från filström med laddningsformat och öppningslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filestream | java.io.InputStream | Strömmen för Excel-filen. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat för Excel-filen. |
| lösenord | java.lang.String | Det öppna lösenordet för Excel-filen. Värdet kan vara null om inget lösenord är angivet. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importerar Excel-filen från filsökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Den fullständiga sökvägen till filen. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Importerar Excel-filen från filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika ID:t för filcachen, om det sätts till null genereras det automatiskt. |
| filestream | java.io.InputStream | Strömmen för Excel-filen. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat för Excel-filen. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Importerar Excel-filen från filström med laddningsformat och öppningslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika ID:t för filcachen, om det sätts till null genereras det automatiskt. |
| filestream | java.io.InputStream | Strömmen för Excel-filen. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). LoadFormat för Excel-filen. |
| lösenord | java.lang.String | Det öppna lösenordet för Excel-filen. Värdet kan vara null om inget lösenord är angivet |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Importerar Excel-filen från filsökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika ID:t för filcachen, om det sätts till null genereras det automatiskt. |
| fileName | java.lang.String | Den fullständiga sökvägen till filen. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Importerar Excel-filen från filsökväg och öppningslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika ID:t för filcachen, om det sätts till null genereras det automatiskt. |
| fileName | java.lang.String | Den fullständiga sökvägen till filen. |
| lösenord | java.lang.String | Det öppna lösenordet för Excel-filen. Värdet kan vara null om inget lösenord är angivet. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Importerar Excel-filen från JSON-formatsträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| json | java.lang.String | JSON-formatsträngen. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Infogar bild i kalkylbladet från filström eller URL (antingen filström eller URL ska tillhandahållas) eller infogar form, när p.type är en av AutoShapeType.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika ID:t för filcachen |
| p | java.lang.String | JSON-formatsträngen för operationen som specificerar cellplatsen, bladnamnet, övre vänstra raden och övre vänstra kolumnen för bilden\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | Filströmmen för bildfilen |
| imageUrl | java.lang.String | URL:en för bildfilen |

**Returns:**
java.lang.String - JSON-formatsträngen för den infogade bilden
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Generera JSON från den minnesbaserade Workbook och skriv den till den angivna strömmen. Cachar valfritt den genererade JSON för snabbare efterföljande hämtning. Viktiga skillnader från JsonToStreamByUid: - Denna metod använder det aktuella minnesbaserade Workbook-tillståndet (wb-fältet) - JsonToStreamByUid laddar om Workbook från .cells-cachefiler på disk - Använd denna metod när du vill exportera det aktuella arbetsbokens tillstånd efter ändringar - Använd JsonToStreamByUid när du behöver återskapa JSON från ett tidigare cachat filtillstånd Caching‑beteende (när uid tillhandahålls): - Kontrollerar JSON-cachen innan generering (L1-minne + L2-disk) - Vid cachemiss genereras JSON från minnesbaserad workbook - Sparar den genererade JSON i cachen för framtida förfrågningar

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Utdataströmmen att skriva JSON-data till |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om den sätts till null, är standardfilnamnet: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| filnamn | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Hämta JSON-strängen för filen från cachen med det angivna unika ID:t, ange utdatafilnamnet i JSON, och skriv den till strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om den sätts till null, är standardfilnamnet: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Hämtar JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| sheetName | java.lang.String | bladnamnet. |

**Returns:**
java.lang.StringBuilder - JSON-sträng StringBuilder
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Hämta JSON-strängen för det angivna bladet i filen från cachen med det angivna unika ID:t, och skriv den till strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| uid | java.lang.String | Det unika id-et för filcachen. |
| sheetName | java.lang.String | bladnamnet. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Tillämpar en batchuppdatering på minnesdata.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| json | java.lang.String | Uppdaterings‑JSON‑formatsträngen. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


Utför radering på en Excel-fil baserat på en array av JSON-operationer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| excelFilePath | java.lang.String | Filvägen till Excel‑filen som ska redigeras. |
| uid | java.lang.String | Den unika identifieraren för arbetsboken. Om null eller tom, genereras ett nytt uid baserat på filsökvägen. |
| arrayOfRedactionOpr | java.lang.String[] | En array av JSON‑strängar som representerar de redigeringsoperationer som ska tillämpas. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Sparar minnesdata till cache-filen med det angivna filnamnet och anger även öppningslösenordet, sparformatet baseras på filändelsen för filnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filnamn | java.lang.String | Filnamnet att spara. |
| lösenord | java.lang.String | Excel‑filens öppningslösenord. Värdet kan vara null om inget lösenord är angivet. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Sparar minnesdata till strömmen, baserat på ursprungsfilformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att spara. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Sparar minnesdata till filsökvägen, om filen har filändelse, sparas formatet baserat på filändelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | Filvägen att spara. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Sparar minnesdata till strömmen, sparformatet är html.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att spara. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Sparar minnesdata till filsökvägen, sparformatet är html.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | Filvägen att spara. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Sparar minnesdata till strömmen, sparformatet är pdf.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att spara. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Sparar minnesdata till filsökvägen, sparformatet är pdf.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | Filvägen att spara. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Sparar minnesdata till strömmen, sparformatet är xlsx.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att spara. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Sparar minnesdata till filsökvägen, sparformatet är xlsx.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | Filvägen att spara. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Ställer in cache‑katalogen för lagring av kalkylbladsfil. Om detta inte är angivet kommer vi att använda den statiska egenskapen från [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) eller [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Ställ in basbildens hämta‑åtgärd‑URL från kontrollern.

**Remarks**

När CacheImp är null måste vi sätta detta.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseImageURL | java.lang.String | Bas‑bildens hämtnings‑URL. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Ställer in InterruptMonitor för laddningsoperationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | InterruptMonitor‑instansen. |
| calculateTimeoutMilliseconds | int | Timeout i millisekunder för att läsa in filen. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Ställer in InterruptMonitor för sparningsoperationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | InterruptMonitor‑instansen. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Representerar arbetsbokens inställningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Ställer in transparensen för redigeringsformer i arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| excelFilePath | java.lang.String | Filsökvägen för Excel‑filen. |
| uid | java.lang.String | Den unika identifieraren för arbetsboken. Om null eller tom, genereras ett nytt uid baserat på filsökvägen. |
| isTransparent | boolean | Om true, sätts transparensen till 0,89 (halvtransparent); om false, sätts transparensen till 1 (fullt ogenomskinlig/osynlig). |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


Översätt alla strängvärden till målspråket i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| sheetName | java.lang.String | Bladnamnet |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Översättaren som implementerar översättningsfunktionen |
| targetLanguage | java.lang.String | Målspråket |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Tillämpar uppdateringsoperationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-formatsträngen för uppdateringsoperationen. |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.String – JSON‑formatsträngen för uppdateringsresultatet.
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

