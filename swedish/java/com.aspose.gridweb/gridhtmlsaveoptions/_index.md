---
title: "GridHtmlSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att spara html-fil."
type: docs
url: /sv/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Representerar alternativen för att spara html-fil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Skapar alternativ för att spara en html-fil. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Skapar alternativ för att spara en htm-fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Den katalog som de bifogade filerna kommer att sparas till. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Ange URL-prefixet för bifogade filer såsom bild i html-filen. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Den cachade filmappen används för att lagra stora data. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getDefaultFontName()](#getDefaultFontName--) | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [getEncoding()](#getEncoding--) | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Anger om hela arbetsboken exporteras till en HTML‑fil. |
| [getExportArea()](#getExportArea--) | Hämtar den exporterade CellArea för det aktuella aktiva kalkylbladet. |
| [getExportGridLines()](#getExportGridLines--) | Anger om rutnätslinjer exporteras. Standardvärdet är false. |
| [getExportHeadings()](#getExportHeadings--) | Anger om rubriker exporteras när filen sparas som HTML. Standardvärdet är false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Anger om endast utskriftsområdet exporteras till HTML-filen. |
| [getExportSingleTab()](#getExportSingleTab--) | Anger om den enda fliken exporteras när filen bara har ett kalkylblad. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getPageTitle()](#getPageTitle--) | Titeln på html-sidan. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Analysera HTML‑tagg i cell, som |

, som cellvärde, eller som HTML‑tagg, standard är true |
| [getPresentationPreference()](#getPresentationPreference--) | Anger om HTML‑ eller MHT‑fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om diagramcachdata uppdateras. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt. |
| [isFullPathLink()](#isFullPathLink--) | Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Den katalog som de bifogade filerna kommer att sparas till. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Ange URL-prefixet för bifogade filer såsom bild i html-filen. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Den cachade filmappen används för att lagra stora data. |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Anger om hela arbetsboken exporteras till en HTML‑fil. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Ställer in exporten av CellArea för det aktuella aktiva kalkylbladet. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Anger om rutnätslinjer exporteras. Standardvärdet är false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Anger om rubriker exporteras när filen sparas som HTML. Standardvärdet är false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Anger om endast utskriftsområdet exporteras till HTML-filen. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Anger om den enda fliken exporteras när filen bara har ett kalkylblad. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Titeln på html-sidan. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Analysera HTML‑tagg i cell, som |

, som cellvärde, eller som HTML‑tagg, standard är true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Anger om HTML‑ eller MHT‑fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om diagramcachdata uppdateras. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Skapar alternativ för att spara en html-fil.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Skapar alternativ för att spara en htm-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Filformatet för sparning. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Katalogen där de bifogade filerna kommer att sparas. Endast för att spara till html‑ström.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Ange Url‑prefixet för bifogade filer, t.ex. bild i html‑filen. Endast för att spara till html‑ström.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Den cachade filmappen används för att lagra stora data.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Gör arbetsboken tom efter att filen har sparats.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Om inte angivet, använd Encoding.UTF8 som standardkodningstyp.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Anger om hela arbetsboken exporteras till en HTML‑fil.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Hämtar exportområdet CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktiva kalkylbladet att utelämnas. Endast det angivna området exporteras när filen sparas som HTML.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Anger om rutnätslinjer exporteras. Standardvärdet är false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Anger om rubriker exporteras när filen sparas som HTML. Standardvärdet är false. Om du vill importera HTML‑filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB.

**Remarks**

När denna egenskap är satt till true exporteras bilddata direkt i img-elementen och separata filer skapas inte.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Anger om endast utskriftsområdet ska exporteras till html‑fil. Standardvärdet är false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Anger om den enda fliken ska exporteras när filen bara har ett arbetsblad. Standardvärdet är false.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Titeln på html‑sidan. Endast för sparande till html‑ström.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Analysera HTML‑tagg i cell, som

, som cellvärde, eller som HTML‑tagg, standard är true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Anger om HTML‑ eller MHT‑fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Anger om diagramcachdata uppdateras.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar filformatet för sparning.

Se [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Anger om definierade namn ska sorteras innan filen sparas.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Anger om sammanslagna celler ska valideras innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false.

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Katalogen där de bifogade filerna kommer att sparas. Endast för att spara till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Ange Url‑prefixet för bifogade filer, t.ex. bild i html‑filen. Endast för att spara till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Den cachade filmappen används för att lagra stora data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Gör arbetsboken tom efter att filen har sparats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Om inte angivet, använd Encoding.UTF8 som standardkodningstyp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Anger om hela arbetsboken exporteras till en HTML‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Ställer in exportområdet CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktiva kalkylbladet att utelämnas. Endast det angivna området exporteras när filen sparas som HTML.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Anger om rutnätslinjer exporteras. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Anger om rubriker exporteras när filen sparas som HTML. Standardvärdet är false. Om du vill importera HTML‑filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB.

**Remarks**

När denna egenskap är satt till true exporteras bilddata direkt i img-elementen och separata filer skapas inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Anger om endast utskriftsområdet ska exporteras till html‑fil. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Anger om den enda fliken ska exporteras när filen bara har ett arbetsblad. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Titeln på html‑sidan. Endast för sparande till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Analysera HTML‑tagg i cell, som

, som cellvärde, eller som HTML‑tagg, standard är true

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Anger om HTML‑ eller MHT‑fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Anger om diagramcachdata uppdateras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Anger om definierade namn ska sorteras innan filen sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Anger om sammanslagna celler ska valideras innan filen sparas.

**Remarks**

Standardvärdet är falskt.

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

