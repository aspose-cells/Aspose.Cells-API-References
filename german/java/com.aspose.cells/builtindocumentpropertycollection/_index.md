---
title: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Eine Sammlung von integrierten Dokumenteigenschaften."
type: docs
url: /de/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

Eine Sammlung von integrierten Dokumenteigenschaften.

**Remarks**

Bietet Zugriff auf Objekte über ihre Namen (unter Verwendung eines Indexers) und über eine Reihe typisierter Eigenschaften, die Werte des entsprechenden Typs zurückgeben.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [clear()](#clear--) | Entfernt alle Objekte aus der CollectionBase-Instanz. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [contains(String name)](#contains-java.lang.String-) | Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach Index zurück. |
| [get(String name)](#get-java.lang.String-) | Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach dem Namen der Eigenschaft zurück. |
| [getAuthor()](#getAuthor--) | Liefert den Namen des Autors des Dokuments. |
| [getBytes()](#getBytes--) | Stellt eine Schätzung der Anzahl von Bytes im Dokument dar. |
| [getCategory()](#getCategory--) | Liefert die Kategorie des Dokuments. |
| [getCharacters()](#getCharacters--) | Stellt eine Schätzung der Anzahl von Zeichen im Dokument dar. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Stellt eine Schätzung der Anzahl von Zeichen (einschließlich Leerzeichen) im Dokument dar. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Liefert die Dokumentkommentare. |
| [getCompany()](#getCompany--) | Liefert die Firmen-Eigenschaft. |
| [getContentStatus()](#getContentStatus--) | Liefert den Inhaltsstatus des Dokuments. |
| [getContentType()](#getContentType--) | Liefert den Inhaltstyp des Dokuments. |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getCreatedTime()](#getCreatedTime--) | Liefert das Erstellungsdatum des Dokuments in der lokalen Zeitzone. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Liefert die universelle Zeit der Dokumenterstellung. |
| [getDocumentVersion()](#getDocumentVersion--) | Stellt die Version der Datei dar. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Liefert die Hyperlinkbase-Eigenschaft. |
| [getKeywords()](#getKeywords--) | Liefert die Dokument-Schlüsselwörter. |
| [getLanguage()](#getLanguage--) | Liefert die Sprache des Dokuments. |
| [getLastPrinted()](#getLastPrinted--) | Liefert das Datum, an dem das Dokument zuletzt in der lokalen Zeitzone gedruckt wurde. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Liefert die universelle Zeit, zu der das Dokument zuletzt gedruckt wurde. |
| [getLastSavedBy()](#getLastSavedBy--) | Liefert den Namen des letzten Autors. |
| [getLastSavedTime()](#getLastSavedTime--) | Liefert die Zeit der letzten Speicherung in der lokalen Zeitzone. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Liefert die universelle Zeit der letzten Speicherung. |
| [getLines()](#getLines--) | Stellt eine Schätzung der Zeilenanzahl im Dokument dar. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Gibt an, ob Hyperlinks in einem Dokument aktuell sind. |
| [getManager()](#getManager--) | Liefert die Manager-Eigenschaft. |
| [getNameOfApplication()](#getNameOfApplication--) | Liefert den Namen der Anwendung. |
| [getPages()](#getPages--) | Stellt eine Schätzung der Seitenanzahl im Dokument dar. |
| [getParagraphs()](#getParagraphs--) | Stellt eine Schätzung der Anzahl der Absätze im Dokument dar. |
| [getRevisionNumber()](#getRevisionNumber--) | Ruft die Dokumentversionsnummer ab. |
| [getScaleCrop()](#getScaleCrop--) | Gibt den Anzeigemodus der Dokumentvorschau an. |
| [getSubject()](#getSubject--) | Ruft den Betreff des Dokuments ab. |
| [getTemplate()](#getTemplate--) | Ruft den Informationsnamen der Dokumentvorlage ab. |
| [getTitle()](#getTitle--) | Ruft den Titel des Dokuments ab. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Ruft die gesamte Bearbeitungszeit in Minuten ab. |
| [getVersion()](#getVersion--) | Stellt die Versionsnummer der Anwendung dar, die das Dokument erstellt hat. |
| [getWords()](#getWords--) | Stellt eine Schätzung der Wortanzahl im Dokument dar. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Ermittelt den Index einer Eigenschaft nach Namen. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung. |
| [removeAt(int index)](#removeAt-int-) | Entfernt eine Eigenschaft am angegebenen Index. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Legt den Namen des Autors des Dokuments fest. |
| [setBytes(int value)](#setBytes-int-) | Stellt eine Schätzung der Anzahl von Bytes im Dokument dar. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Legt die Kategorie des Dokuments fest. |
| [setCharacters(int value)](#setCharacters-int-) | Stellt eine Schätzung der Anzahl von Zeichen im Dokument dar. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Stellt eine Schätzung der Anzahl von Zeichen (einschließlich Leerzeichen) im Dokument dar. |
| [setComments(String value)](#setComments-java.lang.String-) | Legt die Dokumentkommentare fest. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Legt die Firmen-Eigenschaft fest. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Legt den Inhaltsstatus des Dokuments fest. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Legt den Inhaltstyp des Dokuments fest. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Legt das Erstellungsdatum des Dokuments in lokaler Zeitzone fest. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Legt die universelle Zeit der Dokumenterstellung fest. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Stellt die Version der Datei dar. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Legt die Hyperlinkbasis-Eigenschaft fest. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Legt die Dokument-Schlüsselwörter fest. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Legt die Sprache des Dokuments fest. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Legt das Datum fest, an dem das Dokument zuletzt in lokaler Zeitzone gedruckt wurde. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Legt die universelle Zeit fest, zu der das Dokument zuletzt gedruckt wurde. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Legt den Namen des letzten Autors fest. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | Legt die Zeit des letzten Speicherns in lokaler Zeitzone fest. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | Legt die universelle Zeit des letzten Speicherns fest. |
| [setLines(int value)](#setLines-int-) | Stellt eine Schätzung der Zeilenanzahl im Dokument dar. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Gibt an, ob Hyperlinks in einem Dokument aktuell sind. |
| [setManager(String value)](#setManager-java.lang.String-) | Legt die Manager-Eigenschaft fest. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Legt den Namen der Anwendung fest. |
| [setPages(int value)](#setPages-int-) | Stellt eine Schätzung der Seitenanzahl im Dokument dar. |
| [setParagraphs(int value)](#setParagraphs-int-) | Stellt eine Schätzung der Anzahl der Absätze im Dokument dar. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Legt die Revisionsnummer des Dokuments fest. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Gibt den Anzeigemodus der Dokumentvorschau an. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Legt den Betreff des Dokuments fest. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Legt den Informationsnamen der Dokumentvorlage fest. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Legt den Titel des Dokuments fest. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Legt die gesamte Bearbeitungszeit in Minuten fest. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Stellt die Versionsnummer der Anwendung dar, die das Dokument erstellt hat. |
| [setWords(int value)](#setWords-int-) | Stellt eine Schätzung der Wortanzahl im Dokument dar. |
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
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Objekte aus der CollectionBase-Instanz.

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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Gibt true zurück, wenn eine Eigenschaft mit dem angegebenen Namen in der Sammlung existiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der Eigenschaft. |

**Returns:**
boolean - True, wenn die Eigenschaft in der Sammlung existiert; sonst false.
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
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Nullbasierter Index des zu holenden [DocumentProperty](../../com.aspose.cells/documentproperty). |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Gibt ein [DocumentProperty](../../com.aspose.cells/documentproperty)-Objekt nach dem Namen der Eigenschaft zurück.

**Remarks**

Die Zeichenkettennamen der Eigenschaften entsprechen den Namen der typisierten Eigenschaften, die von  verfügbar sind.

Wenn Sie eine Eigenschaft anfordern, die im Dokument nicht vorhanden ist, deren Name jedoch als gültiger integrierter Name erkannt wird, wird eine neue  erstellt, zur Sammlung hinzugefügt und zurückgegeben. Der neu erstellten Eigenschaft wird ein Standardwert zugewiesen (leere Zeichenkette, Null, false oder DateTime.MinValue, abhängig vom Typ der integrierten Eigenschaft).

Wenn Sie eine Eigenschaft anfordern, die im Dokument nicht vorhanden ist und deren Name nicht als integrierter Name erkannt wird, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der abzurufenden Eigenschaft. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Liefert den Namen des Autors des Dokuments.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Stellt eine Schätzung der Anzahl von Bytes im Dokument dar.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Liefert die Kategorie des Dokuments.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Stellt eine Schätzung der Anzahl von Zeichen im Dokument dar.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Stellt eine Schätzung der Anzahl von Zeichen (einschließlich Leerzeichen) im Dokument dar.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


Liefert die Dokumentkommentare.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Liefert die Firmen-Eigenschaft.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Liefert den Inhaltsstatus des Dokuments.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Liefert den Inhaltstyp des Dokuments.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Liefert das Erstellungsdatum des Dokuments in der lokalen Zeitzone.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Liefert die universelle Zeit der Dokumenterstellung.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Stellt die Version der Datei dar.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Liefert die Hyperlinkbase-Eigenschaft.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Liefert die Dokument-Schlüsselwörter.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Liefert die Sprache des Dokuments.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Liefert das Datum, an dem das Dokument zuletzt in der lokalen Zeitzone gedruckt wurde.

**Remarks**

Wenn das Dokument nie gedruckt wurde, gibt diese Eigenschaft DateTime.MinValue zurück.

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Liefert die universelle Zeit, zu der das Dokument zuletzt gedruckt wurde.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Liefert den Namen des letzten Autors.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Liefert die Zeit der letzten Speicherung in der lokalen Zeitzone.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Liefert die universelle Zeit der letzten Speicherung.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Stellt eine Schätzung der Zeilenanzahl im Dokument dar.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Gibt an, ob Hyperlinks in einem Dokument aktuell sind.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Liefert die Manager-Eigenschaft.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Liefert den Namen der Anwendung.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Stellt eine Schätzung der Seitenanzahl im Dokument dar.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Stellt eine Schätzung der Anzahl der Absätze im Dokument dar.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Ruft die Dokumentversionsnummer ab.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Gibt den Anzeigemodus der Dokumentvorschau an.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Ruft den Betreff des Dokuments ab.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Ruft den Informationsnamen der Dokumentvorlage ab.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Ruft den Titel des Dokuments ab.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Ruft die gesamte Bearbeitungszeit in Minuten ab.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Stellt die Versionsnummer der Anwendung dar, die das Dokument erstellt hat.

**Remarks**

Das Format ist "00.0000", zum Beispiel: 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Stellt eine Schätzung der Wortanzahl im Dokument dar.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Ermittelt den Index einer Eigenschaft nach Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der Eigenschaft. |

**Returns:**
int - Der nullbasierte Index. Negativer Wert, wenn nicht gefunden.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Groß-/Kleinschreibung ignorierende Name der Eigenschaft. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt eine Eigenschaft am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Legt den Namen des Autors des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Stellt eine Schätzung der Anzahl von Bytes im Dokument dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Legt die Kategorie des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Stellt eine Schätzung der Anzahl von Zeichen im Dokument dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Stellt eine Schätzung der Anzahl von Zeichen (einschließlich Leerzeichen) im Dokument dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Legt die Dokumentkommentare fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Legt die Firmen-Eigenschaft fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Legt den Inhaltsstatus des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Legt den Inhaltstyp des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Legt das Erstellungsdatum des Dokuments in lokaler Zeitzone fest.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Legt die universelle Zeit der Dokumenterstellung fest.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Stellt die Version der Datei dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Legt die Hyperlinkbasis-Eigenschaft fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Legt die Dokument-Schlüsselwörter fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Legt die Sprache des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Legt das Datum fest, an dem das Dokument zuletzt in lokaler Zeitzone gedruckt wurde.

**Remarks**

Wenn das Dokument nie gedruckt wurde, gibt diese Eigenschaft DateTime.MinValue zurück.

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Legt die universelle Zeit fest, zu der das Dokument zuletzt gedruckt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Legt den Namen des letzten Autors fest.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


Legt die Zeit des letzten Speicherns in lokaler Zeitzone fest.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


Legt die universelle Zeit des letzten Speicherns fest.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Stellt eine Schätzung der Zeilenanzahl im Dokument dar.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Gibt an, ob Hyperlinks in einem Dokument aktuell sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Legt die Manager-Eigenschaft fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Legt den Namen der Anwendung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Stellt eine Schätzung der Seitenanzahl im Dokument dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Stellt eine Schätzung der Anzahl der Absätze im Dokument dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Legt die Revisionsnummer des Dokuments fest.

**Remarks**

Aspose.Cells aktualisiert diese Eigenschaft nicht, wenn Sie das Dokument ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Gibt den Anzeigemodus der Dokumentvorschau an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Legt den Betreff des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Legt den Informationsnamen der Dokumentvorlage fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Legt den Titel des Dokuments fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Legt die gesamte Bearbeitungszeit in Minuten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Stellt die Versionsnummer der Anwendung dar, die das Dokument erstellt hat.

**Remarks**

Das Format ist "00.0000", zum Beispiel: 12.0000

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Stellt eine Schätzung der Wortanzahl im Dokument dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

