---
title: "AbstractGlobalizationSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Globalisierungseinstellungen dar."
type: docs
url: /de/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Stellt die Globalisierungseinstellungen dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Vergleicht zwei Zeichenkettenwerte gemäß bestimmter Sortierregeln. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transformiert die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Vergleicht zwei Zeichenkettenwerte gemäß bestimmter Sortierregeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v1 | java.lang.String | die erste Zeichenkette |
| v2 | java.lang.String | die zweite Zeichenkette |
| ignoreCase | boolean | ob bei Vergleich von Werten die Groß-/Kleinschreibung ignoriert werden soll |

**Returns:**
int - Integer, der die lexikalische Beziehung zwischen den beiden Vergleichswerten angibt
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transformiert die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v | java.lang.String | String-Wert muss mit anderen verglichen werden. |
| ignoreCase | boolean | ob bei Vergleich von Werten die Groß-/Kleinschreibung ignoriert werden soll |

**Returns:**
java.lang.Comparable - Objekt kann verwendet werden, um String-Werte zu vergleichen oder zu sortieren
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

