---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells för Java API-referens"
description: "Implementering för att tillhandahålla sparalternativ som sparar delade delar till filer och sökvägen för den resulterande filen definieras med platshållare."
type: docs
url: /sv/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

Implementering för att tillhandahålla sparalternativ som sparar delade delar till filer och sökvägen för den resulterande filen definieras med platshållare.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Instansierar ett objekt för att tillhandahålla sparalternativ enligt angivna mallar. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Frigir resurser efter bearbetning av den aktuella delade delen. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Om bladindex eller namn alltid ska läggas till i filsökvägen. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Om delningsdelens index alltid ska läggas till i filsökvägen. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Hämtar sparaalternativen som används för att få utdatainställningarna för den aktuella delade delen. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Prefix för indexet för arbetsbladet. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Prefix för indexet för arbetsbladet. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefix för indexet för delningsdelen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Om bladindex eller namn alltid ska läggas till i filsökvägen. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Om delningsdelens index alltid ska läggas till i filsökvägen. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Prefix för indexet för arbetsbladet. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Prefix för indexet för arbetsbladet. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefix för indexet för delningsdelen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


Instansierar ett objekt för att tillhandahålla sparalternativ enligt angivna mallar.

**Remarks**

De stödda platshållarna i filvägsmallen:

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pathTemplate | java.lang.String | Mallen för den resulterande filvägen. |

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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Frigir resurser efter bearbetning av den aktuella delade delen.

**Remarks**

Som standard stänger den här metoden bara strömmen som anges av [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) direkt (om sparaalternativen specificerade en Ström som destination). Användaren kan skriva över den här metoden för att kontrollera hur resurser frigörs enligt deras krav och implementeringen av [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | sparaalternativen som används för den aktuella delade delen. |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Om bladindex eller namn alltid ska läggas till i filvägen. Standardvärdet är false, det vill säga när det bara finns ett blad, kommer bladindex, namn och motsvarande prefix ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) inte att läggas till i filvägen.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Om delningsdelens index alltid ska läggas till i filvägen. Standardvärdet är false, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) inte att läggas till i filvägen.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Hämtar sparaalternativen som används för att få utdatainställningarna för den aktuella delade delen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Om mallen har angetts kommer den skapade instansen att kopiera alla inställningar från den och uppdatera utdatafilen därefter.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


Prefix för indexet för arbetsbladet.

**Remarks**

Om det bara finns ett kalkylblad och [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) är false, kommer detta prefix samt bladindex (eller namn) inte att läggas till i den resulterande filvägen.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


Prefix för indexet för arbetsbladet.

**Remarks**

Om det bara finns ett kalkylblad och [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) är false, kommer detta prefix samt bladindex (eller namn) inte att läggas till i den resulterande filvägen.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Prefix för indexet för delningsdelen.

**Remarks**

Om det bara finns en delningsdel och [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) är false, kommer detta prefix och delningsdelens index (0) inte att läggas till i den resulterande filvägen.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Om bladindex eller namn alltid ska läggas till i filvägen. Standardvärdet är false, det vill säga när det bara finns ett blad, kommer bladindex, namn och motsvarande prefix ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) inte att läggas till i filvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Om delningsdelens index alltid ska läggas till i filvägen. Standardvärdet är false, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) inte att läggas till i filvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Om mallen har angetts kommer den skapade instansen att kopiera alla inställningar från den och uppdatera utdatafilen därefter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


Prefix för indexet för arbetsbladet.

**Remarks**

Om det bara finns ett kalkylblad och [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) är false, kommer detta prefix samt bladindex (eller namn) inte att läggas till i den resulterande filvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


Prefix för indexet för arbetsbladet.

**Remarks**

Om det bara finns ett kalkylblad och [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) är false, kommer detta prefix samt bladindex (eller namn) inte att läggas till i den resulterande filvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Prefix för indexet för delningsdelen.

**Remarks**

Om det bara finns en delningsdel och [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) är false, kommer detta prefix och delningsdelens index (0) inte att läggas till i den resulterande filvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

