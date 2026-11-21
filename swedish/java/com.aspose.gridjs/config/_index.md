---
title: "Config"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla statiska inställningar för GridJs"
type: docs
url: /sv/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

Representerar alla statiska inställningar för GridJs
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Config()](#Config--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Indikerar om klienten ska generera ID istället för det faktiska form‑ID:t i redigeringsrelaterade operationer |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Anger om kolumnbredder ska anpassas automatiskt vid filinläsning. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Anger om radhöjder ska anpassas automatiskt vid filinläsning. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Hämtar om laddningsprestandan automatiskt ska optimeras för kalkylblad med stora celler. |
| [getBaseRouteName()](#getBaseRouteName--) | Hämtar basruttens namn för GridJs‑kontroller‑URL. standardvärdet är "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Hämtar standard maximala kolumn för ett tomt kalkylblad. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Hämtar standard maximala rad för ett tomt kalkylblad. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Hämtar om klient‑side diagramrendering ska aktiveras. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Hämtar cache‑katalogen för lagring av kalkylbladsfil. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Hämtar om det maximala intervallet som inkluderar data, stil, sammanslagna celler och figurer ska visas. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Hämtar om det totala antalet visade figurer/bilder i ett kalkylblad ska begränsas, om satt till true kommer GridJs att begränsa det totala antalet visade figurer eller bilder i ett kalkylblad till MaxShapeOrImageCount, standardvärdet är true. |
| [getJsonCache()](#getJsonCache--) | Hämtar JSON‑cachekonfigurationsalternativ. |
| [getLazyLoading()](#getLazyLoading--) | Hämtar om endast det aktiva kalkylbladet ska laddas, standard är false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Hämtar maximalt antal sekunder för tidsgräns vid sparande till PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Hämtar det totala antalet visade figurer eller bilder i det aktiva bladet, detta gäller när IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Hämtar maximal bredd eller höjd för en figur eller en bild, GridJs kommer att ignorera figuren eller bilden med bredd eller höjd som är större än detta, detta gäller när IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Hämtar det totala antalet visade figurer eller bilder i arbetsboken, detta gäller när IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Hämtar websocket‑destinationerna med prefix "/topic". Standard är "/topic/opr". Används endast i samarbetsläge. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Hämtar cache‑katalogen för bilder. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Hämtar om bilder ska kontrolleras för samma källa, standard är true. Standardvärdet är true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Hämtar om HTML-filen ska sparas som zip-arkiv, standardvärdet är falskt. |
| [getShowChartSheet()](#getShowChartSheet--) | Hämtar om diagrambladet ska visas. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Hämtar om former som är osynliga för UI ska hoppas över, standardvärdet är sant. |
| [getUsePrintArea()](#getUsePrintArea--) | Hämtar om PageSetup.PrintArea ska användas för UI-visningsområdet när kalkylbladet har en PageSetup-inställning för PrintArea. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Hämtar om samarbetsredigering ska stödjas, standardvärdet är falskt. |
| [isWasm()](#isWasm--) | Hämtar om GridJs körs i en webbläsare WebAssembly-värd istället för en serverprocess. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Anger om kolumnbredder ska anpassas automatiskt vid filinläsning. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Anger om radhöjder ska anpassas automatiskt vid filinläsning. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Ställer in om laddningsprestandan automatiskt ska optimeras för kalkylblad med stora celler. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Ställer in basruttens namn för GridJs‑kontroller‑URL. standardvärdet är "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Ställer in om samarbetsredigering ska stödjas, standardvärdet är falskt. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Ställer in standard maximalt antal kolumner för ett tomt kalkylblad. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Ställer in standard maximalt antal rader för ett tomt kalkylblad. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Ställer in om diagramrendering på klientsidan ska aktiveras. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Ställer in cache‑katalogen för lagring av kalkylbladsfil. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Ställer in teckensnittsmappen |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Ställer in teckensnittsmapparna |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Ställer in om det maximala området som inkluderar data, stil, sammanslagna celler och former ska visas. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Ställer in om det totala antalet visade former/bilder i ett kalkylblad ska begränsas, om satt till sant kommer GridJs att begränsa det totala antalet visade former eller bilder i ett kalkylblad till MaxShapeOrImageCount, standardvärdet är sant. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | Ställer in JSON‑cachekonfigurationsalternativ. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Ställer in om endast det aktiva kalkylbladet ska laddas, standardvärdet är falskt. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Ställer in maximalt antal sekunder för timeout vid sparning till PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Ställer in det totala antalet visade former eller bilder i det aktiva bladet, det gäller när IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Ställer in maximal bredd eller höjd för en form eller bild, GridJs kommer att ignorera former eller bilder med bredd eller höjd som överstiger detta, det gäller när IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Ställer in det totala antalet visade former eller bilder i arbetsboken, det gäller när IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Ställer in websocket‑destinationerna med prefix "/topic". standardvärdet är "/topic/opr". Används endast i samarbetsläge. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Ställer in cache‑katalogen för bilder. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Ställer in om det ska kontrolleras om bilder har samma källa, standardvärdet är sant. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Ställer in om HTML-filen ska sparas som zip-arkiv, standardvärdet är falskt. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Ställer in om diagrambladet ska visas. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Ställer in om former som är osynliga för UI ska hoppas över, standardvärdet är sant. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Ställer in om **PageSetup.PrintArea** ska användas för UI:s visningsintervall när kalkylbladet har en PageSetup-inställning för PrintArea. |
| [setWasm(boolean value)](#setWasm-boolean-) | Ställer in om **GridJs** körs i en webbläsar‑WebAssembly‑värd istället för en serverprocess. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
```


Indikerar om klienten ska generera ID istället för det faktiska form‑ID:t i redigeringsrelaterade operationer

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public static boolean getAutoFitColumnsOnLoad()
```


Anger om kolumnbredder ska anpassas automatiskt vid filinläsning. Standardvärdet är `false`. Varning: Att sätta detta till `true` kommer att utföra en automatisk anpassning av alla kolumner efter inläsning, vilket kan ha märkbar påverkan på prestandan.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Anger om radhöjder ska anpassas automatiskt vid filinläsning. Standardvärdet är `false`. Varning: Att sätta detta till `true` kommer att utföra en automatisk anpassning av alla rader efter inläsning, vilket kan ha märkbar påverkan på prestandan.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Hämtar om laddningsprestandan för kalkylblad med stora celler automatiskt ska optimeras. Den kommer att ignorera vissa stilar / kanter för att minska laddningstiden. Standardvärdet är sant.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


Hämtar basruttens namn för GridJs‑kontroller‑URL. standardvärdet är "/GridJs2".

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public static int getEmptySheetMaxCol()
```


Hämtar standard maximalt antal kolumner för ett tomt kalkylblad. Standardvärdet är 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Hämtar standard maximalt antal rader för ett tomt kalkylblad. Standardvärdet är 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


Hämtar om klient‑sidans diagramrendering ska aktiveras. Om den är satt till false, kommer GridJs att endast använda servergenererade diagrambilder/-former. standardvärdet är true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Hämtar cache‑katalogen för lagring av kalkylbladsfilen. Vi måste ange den till en specifik sökväg innan vi använder **GridJs**.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Hämtar om det maximala intervallet som inkluderar data, stil, sammanslagna celler och former ska visas. Om den sista raden eller kolumnen innehåller celler utan värde och formel men med anpassad stil visas inte den raden/kolumnen när detta värde är sant\u9286?\* standardvärdet är sant.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Hämtar om det totala antalet visade figurer/bilder i ett kalkylblad ska begränsas, om satt till true kommer GridJs att begränsa det totala antalet visade figurer eller bilder i ett kalkylblad till MaxShapeOrImageCount, standardvärdet är true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


Hämtar JSON‑cache‑konfigurationsalternativ. Styr både minnes‑ (L1) och disk‑ (L2) cache‑beteende för genererad arbetsbok‑JSON.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Hämtar om endast det aktiva kalkylbladet ska laddas, standard är false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


Hämtar maximalt antal sekunder för timeout vid sparning till PDF. Standardvärdet är 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Hämtar det totala antalet visade former eller bilder i det aktiva bladet, gäller när **IslimitShapeOrImage=true**. Standardvärdet är 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Hämtar maximal bredd eller höjd för en form eller bild, **GridJs** ignorerar former eller bilder med bredd eller höjd som överstiger detta, gäller när **IslimitShapeOrImage=true**. Standardvärdet är 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Hämtar det totala antalet visade former eller bilder i arbetsboken, gäller när **IslimitShapeOrImage=true**. Standardvärdet är 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Hämtar websocket‑destinationerna med prefix "/topic". Standard är "/topic/opr". Används endast i samarbetsläge.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Hämtar cache‑katalogen för bilder. (detta gäller när **GridJsWorkbook.CacheImp** är null) standardvägen blir "\\_piccache" i **FileCacheDirectory**.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Hämtar om bilder ska kontrolleras för samma källa, standard är true. Standardvärdet är true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


Hämtar om HTML-filen ska sparas som zip-arkiv, standardvärdet är falskt.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Hämtar om diagrambladet ska visas. Standardvärdet är falskt.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


Hämtar om former som är osynliga för UI ska hoppas över, standardvärdet är sant.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```


Hämtar om **PageSetup.PrintArea** ska användas för UI:s visningsintervall när kalkylbladet har en PageSetup‑inställning för PrintArea. Standardvärdet är falskt.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public static boolean isCollaborative()
```


Hämtar om samarbetsredigering ska stödjas, standardvärdet är falskt.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


Hämtar om GridJs körs i en webbläsar‑WebAssembly‑värd istället för en serverprocess. När true används ingen FileCacheDirectory / disk / interrupt‑thread‑sökväg och filcachen måste komma från GridJsOptions.CacheImp. GridJsOptions.IsWasm sätter detta när GridJs‑tjänsten konstrueras, så en Aspose.Cells.GridJs.dll kan tjäna båda värdarna. standardvärdet är false.

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




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public static void setAutoFitColumnsOnLoad(boolean value)
```


Anger om kolumnbredder ska anpassas automatiskt vid filinläsning. Standardvärdet är `false`. Varning: Att sätta detta till `true` kommer att utföra en automatisk anpassning av alla kolumner efter inläsning, vilket kan ha märkbar påverkan på prestandan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Anger om radhöjder ska anpassas automatiskt vid filinläsning. Standardvärdet är `false`. Varning: Att sätta detta till `true` kommer att utföra en automatisk anpassning av alla rader efter inläsning, vilket kan ha märkbar påverkan på prestandan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Ställer in om laddningsprestandan för kalkylblad med stora celler automatiskt ska optimeras. Den kommer att ignorera vissa stilar / kanter för att minska laddningstiden. Standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


Ställer in basruttens namn för GridJs‑kontroller‑URL. standardvärdet är "/GridJs2".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Ställer in om samarbetsredigering ska stödjas, standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Ställer in standard maximalt antal kolumner för ett tomt kalkylblad. Standardvärdet är 15.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Ställer in standard maximalt radantal för ett tomt kalkylblad. standardvärdet är 12.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


Ställer in om klient‑sidans diagramrendering ska aktiveras. Om den är satt till false, kommer GridJs att endast använda servergenererade diagrambilder/-former. standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Ställer in cachekatalogen för lagring av kalkylbladsfil. Vi måste ange den till en specifik sökväg innan vi använder GridJs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Ställer in teckensnittsmappen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolder | java.lang.String | Mappen som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Ställer in teckensnittsmapparna

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Mapparna som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Ställer in om det maximala intervallet som inkluderar data, stil, sammanslagna celler och figurer ska visas. Om den sista raden eller kolumnen innehåller celler utan värde och formel men med anpassad stil visas inte den raden/kolumnen när detta värde är true\u9286?\* standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Ställer in om det totala antalet visade former/bilder i ett kalkylblad ska begränsas, om satt till sant kommer GridJs att begränsa det totala antalet visade former eller bilder i ett kalkylblad till MaxShapeOrImageCount, standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


Ställer in JSON-cachekonfigurationsalternativ. Kontrollerar både minnes‑ (L1) och disk‑ (L2) cachebeteende för genererad arbetsbok‑JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Ställer in om endast det aktiva kalkylbladet ska laddas, standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


Ställer in maximalt antal sekunder för timeout vid sparning till PDF. standardvärdet är 10.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Ställer in det totala antalet visade figurer eller bilder i det aktiva bladet, gäller när IslimitShapeOrImage=true. standardvärdet är 100.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Ställer in maximal bredd eller höjd för en figur eller bild, GridJs ignorerar figurer eller bilder med bredd eller höjd som överstiger detta, gäller när IslimitShapeOrImage=true. standardvärdet är 10000.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Ställer in det totala antalet visade figurer eller bilder i arbetsboken, gäller när IslimitShapeOrImage=true. standardvärdet är 300.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Ställer in websocket‑destinationerna med prefix "/topic". standardvärdet är "/topic/opr". Används endast i samarbetsläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Ställer in cachekatalogen för bilder. (detta gäller när GridJsWorkbook.CacheImp är null) standardvägen blir "\_piccache" i FileCacheDirectory.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Ställer in om det ska kontrolleras om bilder har samma källa, standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


Ställer in om HTML-filen ska sparas som zip-arkiv, standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Ställer in om diagrambladet ska visas. standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


Ställer in om former som är osynliga för UI ska hoppas över, standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Ställer in om PageSetup.PrintArea ska användas för UI‑visningsintervallet när kalkylbladet har PageSetup‑inställning för PrintArea. standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


Ställer in om GridJs körs i en webbläsar‑WebAssembly‑värd istället för en serverprocess. När true används ingen FileCacheDirectory / disk / interrupt‑thread‑sökväg och filcachen måste komma från GridJsOptions.CacheImp. GridJsOptions.IsWasm sätter detta när GridJs‑tjänsten konstrueras, så en Aspose.Cells.GridJs.dll kan tjäna båda värdarna. standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

