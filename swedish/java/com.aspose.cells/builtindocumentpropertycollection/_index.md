---
title: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "En samling av inbyggda dokumentegenskaper."
type: docs
url: /sv/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

En samling av inbyggda dokumentegenskaper.

**Remarks**

Tillhandahåller åtkomst till objekt via deras namn (med en indexerare) och via en uppsättning typade egenskaper som returnerar värden av lämpliga typer.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [contains(String name)](#contains-java.lang.String-) | Returnerar true om en egenskap med det angivna namnet finns i samlingen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter index. |
| [get(String name)](#get-java.lang.String-) | Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter egenskapens namn. |
| [getAuthor()](#getAuthor--) | Hämtar namnet på dokumentets författare. |
| [getBytes()](#getBytes--) | Representerar en uppskattning av antalet byte i dokumentet. |
| [getCategory()](#getCategory--) | Hämtar dokumentets kategori. |
| [getCharacters()](#getCharacters--) | Representerar en uppskattning av antalet tecken i dokumentet. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Representerar en uppskattning av antalet tecken (inklusive mellanslag) i dokumentet. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Hämtar dokumentets kommentarer. |
| [getCompany()](#getCompany--) | Hämtar egenskapen företag. |
| [getContentStatus()](#getContentStatus--) | Hämtar dokumentets innehållsstatus. |
| [getContentType()](#getContentType--) | Hämtar dokumentets innehållstyp. |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getCreatedTime()](#getCreatedTime--) | Hämtar datum för dokumentets skapande i lokal tidszon. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Hämtar den universella tiden för dokumentets skapande. |
| [getDocumentVersion()](#getDocumentVersion--) | Representerar filens version. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Hämtar egenskapen hyperlinkbase. |
| [getKeywords()](#getKeywords--) | Hämtar dokumentets nyckelord. |
| [getLanguage()](#getLanguage--) | Hämtar dokumentets språk. |
| [getLastPrinted()](#getLastPrinted--) | Hämtar datumet då dokumentet senast skrevs ut i lokal tidszon. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Hämtar den universella tiden då dokumentet senast skrevs ut. |
| [getLastSavedBy()](#getLastSavedBy--) | Hämtar namnet på den senaste författaren. |
| [getLastSavedTime()](#getLastSavedTime--) | Hämtar tiden för den senaste sparningen i lokal tidszon. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Hämtar den universella tiden för den senaste sparningen. |
| [getLines()](#getLines--) | Representerar en uppskattning av antalet rader i dokumentet. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Indikerar om hyperlänkar i ett dokument är uppdaterade. |
| [getManager()](#getManager--) | Hämtar egenskapen manager. |
| [getNameOfApplication()](#getNameOfApplication--) | Hämtar namnet på applikationen. |
| [getPages()](#getPages--) | Representerar en uppskattning av antalet sidor i dokumentet. |
| [getParagraphs()](#getParagraphs--) | Representerar en uppskattning av antalet stycken i dokumentet. |
| [getRevisionNumber()](#getRevisionNumber--) | Hämtar dokumentets revisionsnummer. |
| [getScaleCrop()](#getScaleCrop--) | Anger visningsläget för dokumentets miniatyrbild. |
| [getSubject()](#getSubject--) | Hämtar dokumentets ämne. |
| [getTemplate()](#getTemplate--) | Hämtar det informativa namnet på dokumentmallen. |
| [getTitle()](#getTitle--) | Hämtar dokumentets titel. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Hämtar den totala redigeringstiden i minuter. |
| [getVersion()](#getVersion--) | Representerar versionsnumret för programmet som skapade dokumentet. |
| [getWords()](#getWords--) | Representerar en uppskattning av antalet ord i dokumentet. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Hämtar index för en egenskap efter namn. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Tar bort en egenskap med det angivna namnet från samlingen. |
| [removeAt(int index)](#removeAt-int-) | Tar bort en egenskap på det angivna indexet. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ställer in namnet på dokumentets författare. |
| [setBytes(int value)](#setBytes-int-) | Representerar en uppskattning av antalet byte i dokumentet. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Ställer in dokumentets kategori. |
| [setCharacters(int value)](#setCharacters-int-) | Representerar en uppskattning av antalet tecken i dokumentet. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Representerar en uppskattning av antalet tecken (inklusive mellanslag) i dokumentet. |
| [setComments(String value)](#setComments-java.lang.String-) | Ställer in dokumentets kommentarer. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Ställer in företagsattributet. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Ställer in innehållsstatus för dokumentet. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Ställer in innehållstypen för dokumentet. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Ställer in datum för dokumentets skapande i lokal tidszon. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Ställer in den universella tiden för dokumentets skapande. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Representerar filens version. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Ställer in egenskapen hyperlinkbase. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Ställer in dokumentets nyckelord. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Ställer in dokumentets språk. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Ställer in datumet då dokumentet senast skrevs ut i lokal tidszon. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Ställer in den universella tiden då dokumentet senast skrevs ut. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Ställer in namnet på den sista författaren. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | Ställer in tiden för den senaste sparningen i lokal tidszon. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | Ställer in den universella tiden för den senaste sparningen. |
| [setLines(int value)](#setLines-int-) | Representerar en uppskattning av antalet rader i dokumentet. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Indikerar om hyperlänkar i ett dokument är uppdaterade. |
| [setManager(String value)](#setManager-java.lang.String-) | Ställer in chefegenskapen. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Ställer in namnet på programmet. |
| [setPages(int value)](#setPages-int-) | Representerar en uppskattning av antalet sidor i dokumentet. |
| [setParagraphs(int value)](#setParagraphs-int-) | Representerar en uppskattning av antalet stycken i dokumentet. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Ställer in dokumentets revisionsnummer. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Anger visningsläget för dokumentets miniatyrbild. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Ställer in dokumentets ämne. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Ställer in det informativa namnet på dokumentmallen. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Ställer in dokumentets titel. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Ställer in total redigeringstid i minuter. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Representerar versionsnumret för programmet som skapade dokumentet. |
| [setWords(int value)](#setWords-int-) | Representerar en uppskattning av antalet ord i dokumentet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från CollectionBase-instansen.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Returnerar true om en egenskap med det angivna namnet finns i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

**Returns:**
boolean - True om egenskapen finns i samlingen; false annars.
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
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Nollbaserat index för den [DocumentProperty](../../com.aspose.cells/documentproperty) som ska hämtas. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter egenskapens namn.

**Remarks**

Strängnamnen på egenskaperna motsvarar namnen på de typade egenskaperna som finns tillgängliga från .

Om du begär en egenskap som inte finns i dokumentet, men egenskapens namn känns igen som ett giltigt inbyggt namn, skapas en ny  , läggs till i samlingen och returneras. Den nyss skapade egenskapen tilldelas ett standardvärde (tom sträng, noll, falskt eller DateTime.MinValue beroende på typen av den inbyggda egenskapen).

Om du begär en egenskap som inte finns i dokumentet och namnet inte känns igen som ett inbyggt namn, returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen som ska hämtas. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Hämtar namnet på dokumentets författare.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Representerar en uppskattning av antalet byte i dokumentet.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Hämtar dokumentets kategori.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Representerar en uppskattning av antalet tecken i dokumentet.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Representerar en uppskattning av antalet tecken (inklusive mellanslag) i dokumentet.

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


Hämtar dokumentets kommentarer.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Hämtar egenskapen företag.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Hämtar dokumentets innehållsstatus.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Hämtar dokumentets innehållstyp.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Hämtar datum för dokumentets skapande i lokal tidszon.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Hämtar den universella tiden för dokumentets skapande.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Representerar filens version.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Hämtar egenskapen hyperlinkbase.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Hämtar dokumentets nyckelord.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Hämtar dokumentets språk.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Hämtar datumet då dokumentet senast skrevs ut i lokal tidszon.

**Remarks**

Om dokumentet aldrig har skrivits ut kommer den här egenskapen att returnera DateTime.MinValue.

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Hämtar den universella tiden då dokumentet senast skrevs ut.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Hämtar namnet på den senaste författaren.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Hämtar tiden för den senaste sparningen i lokal tidszon.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Hämtar den universella tiden för den senaste sparningen.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Representerar en uppskattning av antalet rader i dokumentet.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Indikerar om hyperlänkar i ett dokument är uppdaterade.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Hämtar egenskapen manager.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Hämtar namnet på applikationen.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Representerar en uppskattning av antalet sidor i dokumentet.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Representerar en uppskattning av antalet stycken i dokumentet.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Hämtar dokumentets revisionsnummer.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Anger visningsläget för dokumentets miniatyrbild.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Hämtar dokumentets ämne.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Hämtar det informativa namnet på dokumentmallen.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Hämtar dokumentets titel.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Hämtar den totala redigeringstiden i minuter.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Representerar versionsnumret för programmet som skapade dokumentet.

**Remarks**

Dess format är "00.0000", till exempel: 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Representerar en uppskattning av antalet ord i dokumentet.

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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Hämtar index för en egenskap efter namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

**Returns:**
int - Det nollbaserade indexet. Negativt värde om inte hittat.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Tar bort en egenskap med det angivna namnet från samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort en egenskap på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Ställer in namnet på dokumentets författare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Representerar en uppskattning av antalet byte i dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Ställer in dokumentets kategori.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Representerar en uppskattning av antalet tecken i dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Representerar en uppskattning av antalet tecken (inklusive mellanslag) i dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Ställer in dokumentets kommentarer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Ställer in företagsattributet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Ställer in innehållsstatus för dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Ställer in innehållstypen för dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Ställer in datum för dokumentets skapande i lokal tidszon.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Ställer in den universella tiden för dokumentets skapande.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Representerar filens version.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Ställer in egenskapen hyperlinkbase.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Ställer in dokumentets nyckelord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Ställer in dokumentets språk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Ställer in datumet då dokumentet senast skrevs ut i lokal tidszon.

**Remarks**

Om dokumentet aldrig har skrivits ut kommer den här egenskapen att returnera DateTime.MinValue.

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Ställer in den universella tiden då dokumentet senast skrevs ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Ställer in namnet på den sista författaren.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


Ställer in tiden för den senaste sparningen i lokal tidszon.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


Ställer in den universella tiden för den senaste sparningen.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Representerar en uppskattning av antalet rader i dokumentet.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Indikerar om hyperlänkar i ett dokument är uppdaterade.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Ställer in chefegenskapen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Ställer in namnet på programmet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Representerar en uppskattning av antalet sidor i dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Representerar en uppskattning av antalet stycken i dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Ställer in dokumentets revisionsnummer.

**Remarks**

Aspose.Cells uppdaterar inte den här egenskapen när du ändrar dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Anger visningsläget för dokumentets miniatyrbild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Ställer in dokumentets ämne.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Ställer in det informativa namnet på dokumentmallen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Ställer in dokumentets titel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Ställer in total redigeringstid i minuter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Representerar versionsnumret för programmet som skapade dokumentet.

**Remarks**

Dess format är "00.0000", till exempel: 12.0000

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Representerar en uppskattning av antalet ord i dokumentet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

