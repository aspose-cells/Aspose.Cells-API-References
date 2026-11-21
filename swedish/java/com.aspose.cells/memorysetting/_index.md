---
title: "MemorySetting"
second_title: "Aspose.Cells för Java API-referens"
description: "Minnesanvändningslägen för cellernas datamodell."
type: docs
url: /sv/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Minnesanvändningslägen för cellernas datamodell.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Minnesprestanda föredras och att använda fil istället för minne för att lagra celldata. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Minnesprestanda föredras. |
| [NORMAL](#NORMAL) | Standardläge för cellmodellen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


Minnesprestanda föredras och att använda fil istället för minne för att lagra celldata.

**Remarks**

Med detta läge kommer celldata att hållas i kompakt format och den största delen av data kommer att lagras i en temporär fil istället för i minnet. Så när man jämför med läget [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) kan detta läge minska minneskostnaden mer, men I/O‑operationerna för att komma åt celldata kommer också att medföra högre tidskostnad.

Detta alternativ är tillgängligt sedan v25.7.0.

| Vissa anmärkningsvärda begränsningar och rekommenderade operationer när detta läge används: |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| När detta läge används för ett kalkylblad i en arbetsbok, bör [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) anropas i slutet av arbetet för att frigöra alla resurser såsom temporära filer. |
| Slumpmässig åtkomst till celler ger dålig prestanda eftersom data måste läsas slumpmässigt och upprepade gånger (så pekaren i filen ändras därefter och I/O‑operationer krävs upprepade gånger). Om möjligt, vänligen åtkom data sekventiellt (rad för rad). |
| När data i en rad/cell ändras kan data i andra celler/rader också påverkas (t.ex. att data flyttas till andra platser för att skapa tillräckligt utrymme för den ändrade datan). Så varje förändring av varje data kräver synkronisering av andra befintliga objekt (såsom Rad‑ eller Cell‑objekt). För att få bättre prestanda, vänligen håll inte flera Rader/Cellar samtidigt. Att bearbeta dem en i taget minskar datasynkroniseringen och prestandan kan förbättras. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Minnesprestanda föredras.

**Remarks**

Med detta läge kommer celldata att hållas i kompakt format för att minska minneskostnaden. Å andra sidan kan den kompakta datan också medföra högre tidskostnad, särskilt vid uppdatering av celldata eller vid slumpmässig åtkomst.

Detta alternativ är tillgängligt sedan v8.0.0.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Standardläge för cellmodellen.

**Remarks**

Det här läget tillämpas för alla versioner.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

