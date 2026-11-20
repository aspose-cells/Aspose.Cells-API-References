---
title: "FontSettingCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Liste von . dar."
type: docs
url: /de/java/com.aspose.cells/fontsettingcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```

Stellt die Liste von [FontSetting](../../com.aspose.cells/fontsetting) dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [appendText(String text)](#appendText-java.lang.String-) | Fügt den Text an. |
| [clear()](#clear--) | Alle Einstellungen löschen. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [deleteText(int index, int count)](#deleteText-int-int-) | Einige Zeichen löschen. |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatiere den Text mit der Schrifteinstellung. |
| [get(int index)](#get-int-) | Ruft das [FontSetting](../../com.aspose.cells/fontsetting) nach dem Index ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getHtmlString()](#getHtmlString--) | Ruft die HTML-Zeichenkette ab, die Daten und einige Formate in dieser Form enthält. |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | Ruft den Enumerator der Absätze ab. |
| [getText()](#getText--) | Ruft den Text der Form ab. |
| [getTextAlignment()](#getTextAlignment--) | Stellt die Ausrichtungseinstellung des Textkörpers dar. |
| [getTextParagraphs()](#getTextParagraphs--) | Ruft alle Absätze ab. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Fügt den Index an der Position ein. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element am angegebenen Index. |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | Ersetze den Text. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersetze den Text. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Setzt die HTML-Zeichenkette, die Daten und einige Formate in dieser Form enthält. |
| [setText(String value)](#setText-java.lang.String-) | Setzt den Text der Form. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Legt den vordefinierten WordArt-Stil fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```


Fügt den Text an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Der Text. |

### clear() {#clear--}
```
public void clear()
```


Alle Einstellungen löschen.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```


Einige Zeichen löschen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Startindex. |
| Anzahl | int | Die Anzahl der Zeichen. |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```


Formatiere den Text mit der Schrifteinstellung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |
| length | int | Die Länge. |
| font | [Font](../../com.aspose.cells/font) | Die Schriftart. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Die Flags der Schriftart. |

### get(int index) {#get-int-}
```
public FontSetting get(int index)
```


Ruft das [FontSetting](../../com.aspose.cells/fontsetting) nach dem Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Ruft die HTML-Zeichenkette ab, die Daten und einige Formate in dieser Form enthält.

**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```


Ruft den Enumerator der Absätze ab.

**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```


Ruft den Text der Form ab.

**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```


Stellt die Ausrichtungseinstellung des Textkörpers dar.

**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```


Ruft alle Absätze ab.

**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Fügt den Index an der Position ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Startindex. |
| Text | java.lang.String | Der Text. |

### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des zu entfernenden Elements. |

### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```


Ersetze den Text.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Startindex. |
| Anzahl | int | Die Anzahl der Zeichen. |
| Text | java.lang.String | Der Text. |

### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```


Ersetze den Text.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | java.lang.String | Der alte Text. |
| newValue | java.lang.String | Der neue Text. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Setzt die HTML-Zeichenkette, die Daten und einige Formate in dieser Form enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Setzt den Text der Form.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Legt den vordefinierten WordArt-Stil fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Der voreingestellte WordArt-Stil. |

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

