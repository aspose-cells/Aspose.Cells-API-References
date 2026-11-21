---
title: "ReConnectionMethodType"
second_title: "Aspose.Cells för Java API-referens"
description: "Specificerar vad kalkylbladsapplikationen ska göra när en anslutning misslyckas."
type: docs
url: /sv/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

Specificerar vad kalkylbladsapplikationen ska göra när en anslutning misslyckas.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ALWAYS](#ALWAYS) | Vid varje uppdatering hämta uppdaterad anslutningsinformation från den externa anslutningsfilen, om den finns tillgänglig, och använd den i stället för den befintliga anslutningsinformationen. |
| [NEVER](#NEVER) | Hämta aldrig uppdaterad anslutningsinformation från den externa anslutningsfilen även om den är tillgänglig och även om den befintliga anslutningsinformationen är ogiltig. |
| [REQUIRED](#REQUIRED) | Vid uppdatering, använd den befintliga anslutningsinformationen och om den visar sig vara ogiltig, hämta då uppdaterad anslutningsinformation, om den finns tillgänglig i den externa anslutningsfilen. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Vid varje uppdatering hämta uppdaterad anslutningsinformation från den externa anslutningsfilen, om den finns tillgänglig, och använd den i stället för den befintliga anslutningsinformationen. I detta fall kommer datauppdateringen att misslyckas om den externa anslutningsfilen är otillgänglig.

### NEVER {#NEVER}
```
public static final int NEVER
```


Hämta aldrig uppdaterad anslutningsinformation från den externa anslutningsfilen även om den är tillgänglig och även om den befintliga anslutningsinformationen är ogiltig.

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


Vid uppdatering, använd den befintliga anslutningsinformationen och om den visar sig vara ogiltig, hämta då uppdaterad anslutningsinformation, om den finns tillgänglig i den externa anslutningsfilen.

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

