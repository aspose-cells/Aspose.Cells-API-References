---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells för Java API-referens"
description: "Implementering för att tillhandahålla sparalternativ som sparar delade delar till filer och sökvägen för den resulterande filen namnges så att den kan innehålla kataloger SheetIndex eller SheetName SplitPartIndex."
type: docs
url: /sv/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Implementering för att tillhandahålla sparalternativ som sparar delade delar till filer och sökvägen för den resulterande filen namnges som (den kan innehålla kataloger): [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(or SheetName) +[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Frigir resurser efter bearbetning av den aktuella delade delen. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Om bladindex eller namn alltid ska läggas till i filsökvägen. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Om delningsdelens index alltid ska läggas till i filsökvägen. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Huvuddel (före tillagt innehåll för blad och del) av filsökvägen. |
| [getPathTail()](#getPathTail--) | Avslutningsdel (efter sekvensnummer) av filsökvägen. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Hämtar sparaalternativen som används för att få utdatainställningarna för den aktuella delade delen. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Prefix för indexet för arbetsbladet. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefix för indexet för delningsdelen. |
| [getUseSheetName()](#getUseSheetName--) | Om filsökvägen byggs med bladnamn istället för bladindex. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Om bladindex eller namn alltid ska läggas till i filsökvägen. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Om delningsdelens index alltid ska läggas till i filsökvägen. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Huvuddel (före tillagt innehåll för blad och del) av filsökvägen. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Avslutningsdel (efter sekvensnummer) av filsökvägen. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Prefix för indexet för arbetsbladet. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefix för indexet för delningsdelen. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Om filsökvägen byggs med bladnamn istället för bladindex. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
```


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


Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är false, det vill säga när det bara finns ett blad, kommer bladindex (eller namn) och motsvarande prefix inte att läggas till i filsökvägen.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Om delningsdelens index alltid ska läggas till i filsökvägen. Standardvärdet är false, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix inte att läggas till i filsökvägen.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Huvuddel (före tillagt innehåll för blad och del) av filsökvägen.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Avslutningsdel (efter sekvensnummer) av filsökvägen. Den bör inkludera filnamnets filändelse.

**Returns:**
java.lang.String
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


Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Om mallen har angetts kommer den skapade instansen att kopiera alla inställningar från den och uppdatera utdatafilen därefter.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Gäller endast när [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) är false.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Prefix för indexet för arbetsbladet.

**Remarks**

Om det bara finns ett arbetsblad och [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) är false, kommer detta prefix och bladindex (eller namn) inte att läggas till i den resulterande filsökvägen.

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

Om det bara finns en delningsdel och [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) är false, kommer detta prefix och delningsdelens index (0) inte att läggas till i den resulterande filsökvägen.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Om filvägen byggs med bladnamn istället för bladindex. Standardvärdet är falskt.

**Remarks**

Bladnamnet kommer aldrig att byggas om automatiskt. Så när du sätter det till true, se till att det inte finns något speciellt bladnamn som kan orsaka ogiltig filväg eller namn.

**Returns:**
boolean
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


Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är false, det vill säga när det bara finns ett blad, kommer bladindex (eller namn) och motsvarande prefix inte att läggas till i filsökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Om delningsdelens index alltid ska läggas till i filsökvägen. Standardvärdet är false, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix inte att läggas till i filsökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Huvuddel (före tillagt innehåll för blad och del) av filsökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Avslutningsdel (efter sekvensnummer) av filsökvägen. Den bör inkludera filnamnets filändelse.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Mallen för att skapa en instans av sparalternativ i [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

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

**Remarks**

Gäller endast när [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Prefix för indexet för arbetsbladet.

**Remarks**

Om det bara finns ett arbetsblad och [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) är false, kommer detta prefix och bladindex (eller namn) inte att läggas till i den resulterande filsökvägen.

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

Om det bara finns en delningsdel och [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) är false, kommer detta prefix och delningsdelens index (0) inte att läggas till i den resulterande filsökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Om filvägen byggs med bladnamn istället för bladindex. Standardvärdet är falskt.

**Remarks**

Bladnamnet kommer aldrig att byggas om automatiskt. Så när du sätter det till true, se till att det inte finns något speciellt bladnamn som kan orsaka ogiltig filväg eller namn.

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

