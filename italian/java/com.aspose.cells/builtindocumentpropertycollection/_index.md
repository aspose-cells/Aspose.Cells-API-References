---
title: "BuiltInDocumentPropertyCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Una raccolta di proprietà del documento integrate."
type: docs
url: /it/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

Una raccolta di proprietà del documento integrate.

**Remarks**

Fornisce l'accesso agli oggetti per nome (utilizzando un indicizzatore) e tramite un insieme di proprietà tipizzate che restituiscono valori dei tipi appropriati.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [contains(String name)](#contains-java.lang.String-) | Restituisce true se una proprietà con il nome specificato esiste nella collezione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per indice. |
| [get(String name)](#get-java.lang.String-) | Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per il nome della proprietà. |
| [getAuthor()](#getAuthor--) | Ottiene il nome dell'autore del documento. |
| [getBytes()](#getBytes--) | Rappresenta una stima del numero di byte nel documento. |
| [getCategory()](#getCategory--) | Ottiene la categoria del documento. |
| [getCharacters()](#getCharacters--) | Rappresenta una stima del numero di caratteri nel documento. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Rappresenta una stima del numero di caratteri (spazi inclusi) nel documento. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Ottiene i commenti del documento. |
| [getCompany()](#getCompany--) | Ottiene la proprietà azienda. |
| [getContentStatus()](#getContentStatus--) | Ottiene lo stato del contenuto del documento. |
| [getContentType()](#getContentType--) | Ottiene il tipo di contenuto del documento. |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [getCreatedTime()](#getCreatedTime--) | Ottiene la data di creazione del documento nel fuso orario locale. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Ottiene l'ora universale della creazione del documento. |
| [getDocumentVersion()](#getDocumentVersion--) | Rappresenta la versione del file. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Ottiene la proprietà hyperlinkbase. |
| [getKeywords()](#getKeywords--) | Ottiene le parole chiave del documento. |
| [getLanguage()](#getLanguage--) | Ottiene la lingua del documento. |
| [getLastPrinted()](#getLastPrinted--) | Ottiene la data in cui il documento è stato stampato l'ultima volta nel fuso orario locale. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Ottiene l'ora universale in cui il documento è stato stampato l'ultima volta. |
| [getLastSavedBy()](#getLastSavedBy--) | Ottiene il nome dell'ultimo autore. |
| [getLastSavedTime()](#getLastSavedTime--) | Ottiene l'ora dell'ultimo salvataggio nel fuso orario locale. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Ottiene l'ora universale dell'ultimo salvataggio. |
| [getLines()](#getLines--) | Rappresenta una stima del numero di righe nel documento. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Indica se i collegamenti ipertestuali in un documento sono aggiornati. |
| [getManager()](#getManager--) | Ottiene la proprietà manager. |
| [getNameOfApplication()](#getNameOfApplication--) | Ottiene il nome dell'applicazione. |
| [getPages()](#getPages--) | Rappresenta una stima del numero di pagine nel documento. |
| [getParagraphs()](#getParagraphs--) | Rappresenta una stima del numero di paragrafi nel documento. |
| [getRevisionNumber()](#getRevisionNumber--) | Ottiene il numero di revisione del documento. |
| [getScaleCrop()](#getScaleCrop--) | Indica la modalità di visualizzazione della miniatura del documento. |
| [getSubject()](#getSubject--) | Ottiene l'oggetto del documento. |
| [getTemplate()](#getTemplate--) | Ottiene il nome informativo del modello di documento. |
| [getTitle()](#getTitle--) | Ottiene il titolo del documento. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Ottiene il tempo totale di modifica in minuti. |
| [getVersion()](#getVersion--) | Rappresenta il numero di versione dell'applicazione che ha creato il documento. |
| [getWords()](#getWords--) | Rappresenta una stima del numero di parole nel documento. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Ottiene l'indice di una proprietà per nome. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Rimuove una proprietà con il nome specificato dalla collezione. |
| [removeAt(int index)](#removeAt-int-) | Rimuove una proprietà all'indice specificato. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Imposta il nome dell'autore del documento. |
| [setBytes(int value)](#setBytes-int-) | Rappresenta una stima del numero di byte nel documento. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Imposta la categoria del documento. |
| [setCharacters(int value)](#setCharacters-int-) | Rappresenta una stima del numero di caratteri nel documento. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Rappresenta una stima del numero di caratteri (spazi inclusi) nel documento. |
| [setComments(String value)](#setComments-java.lang.String-) | Imposta i commenti del documento. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Imposta la proprietà company. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Imposta lo stato del contenuto del documento. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Imposta il tipo di contenuto del documento. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Imposta la data di creazione del documento nel fuso orario locale. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Imposta l'ora universale di creazione del documento. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Rappresenta la versione del file. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Imposta la proprietà hyperlinkbase. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Imposta le parole chiave del documento. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Imposta la lingua del documento. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Imposta la data in cui il documento è stato stampato l'ultima volta nel fuso orario locale. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Imposta l'ora universale in cui il documento è stato stampato l'ultima volta. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Imposta il nome dell'ultimo autore. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | Imposta l'ora dell'ultimo salvataggio nel fuso orario locale. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | Imposta l'ora universale dell'ultimo salvataggio. |
| [setLines(int value)](#setLines-int-) | Rappresenta una stima del numero di righe nel documento. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Indica se i collegamenti ipertestuali in un documento sono aggiornati. |
| [setManager(String value)](#setManager-java.lang.String-) | Imposta la proprietà manager. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Imposta il nome dell'applicazione. |
| [setPages(int value)](#setPages-int-) | Rappresenta una stima del numero di pagine nel documento. |
| [setParagraphs(int value)](#setParagraphs-int-) | Rappresenta una stima del numero di paragrafi nel documento. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Imposta il numero di revisione del documento. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Indica la modalità di visualizzazione della miniatura del documento. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Imposta l'oggetto del documento. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Imposta il nome informativo del modello di documento. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Imposta il titolo del documento. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Imposta il tempo totale di modifica in minuti. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Rappresenta il numero di versione dell'applicazione che ha creato il documento. |
| [setWords(int value)](#setWords-int-) | Rappresenta una stima del numero di parole nel documento. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli oggetti dall'istanza di CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Restituisce true se una proprietà con il nome specificato esiste nella collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

**Returns:**
boolean - True se la proprietà esiste nella collezione; false altrimenti.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | Indice basato su zero del [DocumentProperty](../../com.aspose.cells/documentproperty) da recuperare. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Restituisce un oggetto [DocumentProperty](../../com.aspose.cells/documentproperty) per il nome della proprietà.

**Remarks**

I nomi stringa delle proprietà corrispondono ai nomi delle proprietà tipizzate disponibili da .

Se richiedi una proprietà che non è presente nel documento, ma il nome della proprietà è riconosciuto come un nome incorporato valido, viene creata una nuova  , aggiunta alla collezione e restituita. Alla proprietà appena creata viene assegnato un valore predefinito (stringa vuota, zero, false o DateTime.MinValue a seconda del tipo della proprietà incorporata).

Se richiedi una proprietà che non è presente nel documento e il nome non è riconosciuto come un nome incorporato, viene restituito null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole, da recuperare. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Ottiene il nome dell'autore del documento.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Rappresenta una stima del numero di byte nel documento.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Ottiene la categoria del documento.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Rappresenta una stima del numero di caratteri nel documento.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Rappresenta una stima del numero di caratteri (spazi inclusi) nel documento.

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


Ottiene i commenti del documento.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Ottiene la proprietà azienda.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Ottiene lo stato del contenuto del documento.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Ottiene il tipo di contenuto del documento.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Ottiene la data di creazione del documento nel fuso orario locale.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Ottiene l'ora universale della creazione del documento.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Rappresenta la versione del file.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Ottiene la proprietà hyperlinkbase.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Ottiene le parole chiave del documento.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Ottiene la lingua del documento.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Ottiene la data in cui il documento è stato stampato l'ultima volta nel fuso orario locale.

**Remarks**

Se il documento non è mai stato stampato, questa proprietà restituirà DateTime.MinValue.

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Ottiene l'ora universale in cui il documento è stato stampato l'ultima volta.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Ottiene il nome dell'ultimo autore.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Ottiene l'ora dell'ultimo salvataggio nel fuso orario locale.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Ottiene l'ora universale dell'ultimo salvataggio.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Rappresenta una stima del numero di righe nel documento.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Indica se i collegamenti ipertestuali in un documento sono aggiornati.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Ottiene la proprietà manager.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Ottiene il nome dell'applicazione.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Rappresenta una stima del numero di pagine nel documento.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Rappresenta una stima del numero di paragrafi nel documento.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Ottiene il numero di revisione del documento.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Indica la modalità di visualizzazione della miniatura del documento.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Ottiene l'oggetto del documento.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Ottiene il nome informativo del modello di documento.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Ottiene il titolo del documento.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Ottiene il tempo totale di modifica in minuti.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Rappresenta il numero di versione dell'applicazione che ha creato il documento.

**Remarks**

Il suo formato è "00.0000", per esempio: 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Rappresenta una stima del numero di parole nel documento.

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


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Ottiene l'indice di una proprietà per nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

**Returns:**
int - L'indice basato su zero. Valore negativo se non trovato.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
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


Rimuove una proprietà con il nome specificato dalla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove una proprietà all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Imposta il nome dell'autore del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Rappresenta una stima del numero di byte nel documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Imposta la categoria del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Rappresenta una stima del numero di caratteri nel documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Rappresenta una stima del numero di caratteri (spazi inclusi) nel documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Imposta i commenti del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Imposta la proprietà company.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Imposta lo stato del contenuto del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Imposta il tipo di contenuto del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Imposta la data di creazione del documento nel fuso orario locale.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Imposta l'ora universale di creazione del documento.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Rappresenta la versione del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Imposta la proprietà hyperlinkbase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Imposta le parole chiave del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Imposta la lingua del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Imposta la data in cui il documento è stato stampato l'ultima volta nel fuso orario locale.

**Remarks**

Se il documento non è mai stato stampato, questa proprietà restituirà DateTime.MinValue.

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Imposta l'ora universale in cui il documento è stato stampato l'ultima volta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Imposta il nome dell'ultimo autore.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


Imposta l'ora dell'ultimo salvataggio nel fuso orario locale.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


Imposta l'ora universale dell'ultimo salvataggio.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Rappresenta una stima del numero di righe nel documento.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Indica se i collegamenti ipertestuali in un documento sono aggiornati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Imposta la proprietà manager.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Imposta il nome dell'applicazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Rappresenta una stima del numero di pagine nel documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Rappresenta una stima del numero di paragrafi nel documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Imposta il numero di revisione del documento.

**Remarks**

Aspose.Cells non aggiorna questa proprietà quando modifichi il documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Indica la modalità di visualizzazione della miniatura del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Imposta l'oggetto del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Imposta il nome informativo del modello di documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Imposta il titolo del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Imposta il tempo totale di modifica in minuti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Rappresenta il numero di versione dell'applicazione che ha creato il documento.

**Remarks**

Il suo formato è "00.0000", per esempio: 12.0000

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Rappresenta una stima del numero di parole nel documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

