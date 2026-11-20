---
title: "AbstractLowCodeProtectionProvider"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Implementierung zur Bereitstellung von Schutzeinstellungen"
type: docs
url: /de/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Implementierung zur Bereitstellung von Schutzeinstellungen
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Liefert das Passwort zum Öffnen der Tabellenkalkulationsdatei. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Liefert das Passwort zum Schützen der Arbeitsmappe mit dem angegebenen Schutztyp. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Liefert den Schutztyp zum Schützen der Arbeitsmappe. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Liefert das Passwort zum Schützen des angegebenen Arbeitsblatts. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Liefert den Schutztyp zum Schützen des angegebenen Arbeitsblatts. |
| [getWritePassword()](#getWritePassword--) | Liefert das Passwort zum Ändern der Tabellenkalkulationsdatei. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


Liefert das Passwort zum Öffnen der Tabellenkalkulationsdatei.

**Returns:**
java.lang.String - Passwort zum Öffnen der Tabellenkalkulationsdatei. Leer bedeutet keinen Schutz beim Öffnen der Datei.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Liefert das Passwort zum Schützen der Arbeitsmappe mit dem angegebenen Schutztyp.

**Returns:**
java.lang.String - Passwort zum Schützen der Arbeitsmappe.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Liefert den Schutztyp zum Schützen der Arbeitsmappe.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Schutztyp zum Schützen der Arbeitsmappe. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) bedeutet keinen Schutz für die Arbeitsmappe.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Liefert das Passwort zum Schützen des angegebenen Arbeitsblatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Passwort zum Schützen des angegebenen Arbeitsblatts.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Liefert den Schutztyp zum Schützen des angegebenen Arbeitsblatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Schutztyp zum Schützen des angegebenen Arbeitsblatts. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) bedeutet keinen Schutz für das Arbeitsblatt.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Liefert das Passwort zum Ändern der Tabellenkalkulationsdatei.

**Returns:**
java.lang.String - Passwort zum Ändern der Tabellenkalkulationsdatei. Leer bedeutet keinen Schutz beim Ändern der Datei.
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

