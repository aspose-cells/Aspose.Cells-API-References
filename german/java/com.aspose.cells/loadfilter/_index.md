---
title: "LoadFilter"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Filter dar, der Optionen zum Laden von Daten beim Laden einer Arbeitsmappe aus einer Vorlage bereitstellt."
type: docs
url: /de/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Stellt den Filter dar, der Optionen zum Laden von Daten beim Laden einer Arbeitsmappe aus einer Vorlage bereitstellt.

**Remarks**

Der Benutzer kann die Filteroptionen angeben oder sein eigenes LoadFilter implementieren, um festzulegen, wie Daten geladen werden.

**Example**

Das folgende Beispiel zeigt, wie die Filteroptionen anhand der Eigenschaften des Arbeitsblatts bestimmt werden.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Erstellt ein LoadFilter mit den Standardfilteroptionen LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Erstellt ein LoadFilter mit den angegebenen Filteroptionen. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Die Filteroptionen, die angeben, welche Daten geladen werden sollen. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Gibt die zu ladenden Tabellen (Indizes) und deren Reihenfolge an. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Die Filteroptionen, die angeben, welche Daten geladen werden sollen. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Bereitet die Filteroptionen vor, bevor das angegebene Arbeitsblatt geladen wird. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Erstellt ein LoadFilter mit den Standardfilteroptionen LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Erstellt ein LoadFilter mit den angegebenen Filteroptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). die Standardfilteroptionen |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Die Filteroptionen, die angeben, welche Daten geladen werden sollen.

Siehe [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Gibt die zu ladenden Tabellen (Indizes) und deren Reihenfolge an. Standard ist null, was bedeutet, dass alle Tabellen in der Standardreihenfolge der Vorlagendatei geladen werden. Wenn nicht null und der Index einer Tabelle nicht im zurückgegebenen Array enthalten ist, wird diese Tabelle nicht geladen.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Die Filteroptionen, die angeben, welche Daten geladen werden sollen.

Siehe [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Bereitet die Filteroptionen vor, bevor das angegebene Arbeitsblatt geladen wird. Die Implementierung des LoadFilter durch den Benutzer kann hier die LoadDataFilterOptions ändern, um festzulegen, wie Daten für dieses Arbeitsblatt geladen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Das zu ladende Arbeitsblatt. Es können hier nur wenige Eigenschaften des angegebenen Arbeitsblattobjekts verwendet werden, da die meisten Daten und Eigenschaften noch nicht geladen wurden. Die verfügbaren Eigenschaften sind: Name, Index, VisibilityType. |

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

