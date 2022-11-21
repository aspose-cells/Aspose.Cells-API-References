---
title: BuiltInDocumentPropertyCollection
second_title: Aspose.Cells for Java API Reference
description: A collection of built-in document properties.
type: docs
weight: 44
url: /java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

A collection of built-in document properties.

Provides access to  objects by their names (using an indexer) and via a set of typed properties that return values of appropriate types.
## Constructors

| Constructor | Description |
| --- | --- |
| [BuiltInDocumentPropertyCollection()](#BuiltInDocumentPropertyCollection--) |  |
## Methods

| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [contains(String name)](#contains-java.lang.String-) | Returns true if a property with the specified name exists in the collection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by index. |
| [get(String name)](#get-java.lang.String-) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by the name of the property. |
| [getAuthor()](#getAuthor--) | Gets or sets the name of the document's author. |
| [getBytes()](#getBytes--) | Represents an estimate of the number of bytes in the document. |
| [getCategory()](#getCategory--) | Gets or sets the category of the document. |
| [getCharacters()](#getCharacters--) | Represents an estimate of the number of characters in the document. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Represents an estimate of the number of characters (including spaces) in the document. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Gets or sets the document comments. |
| [getCompany()](#getCompany--) | Gets or sets the company property. |
| [getContentStatus()](#getContentStatus--) | Gets or sets the content status of the document. |
| [getContentType()](#getContentType--) | Gets or sets the content type of the document. |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [getCreatedTime()](#getCreatedTime--) | Gets or sets date of the document creation in local timezone. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Gets or sets the Universal time of the document creation. |
| [getDocumentVersion()](#getDocumentVersion--) | Represents the version of the file. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Gets or sets the hyperlinkbase property. |
| [getKeywords()](#getKeywords--) | Gets or sets the document keywords. |
| [getLanguage()](#getLanguage--) | Gets or sets the document's language. |
| [getLastPrinted()](#getLastPrinted--) | Gets or sets the date when the document was last printed in local timezone. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Gets or sets the Universal time when the document was last printed. |
| [getLastSavedBy()](#getLastSavedBy--) | Gets or sets the name of the last author. |
| [getLastSavedTime()](#getLastSavedTime--) | Gets or sets the time of the last save in local timezone. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Gets or sets the universal time of the last save. |
| [getLines()](#getLines--) | Represents an estimate of the number of lines in the document. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Indicates whether hyperlinks in a document are up-to-date. |
| [getManager()](#getManager--) | Gets or sets the manager property. |
| [getNameOfApplication()](#getNameOfApplication--) | Gets or sets the name of the application. |
| [getPages()](#getPages--) | Represents an estimate of the number of pages in the document. |
| [getParagraphs()](#getParagraphs--) | Represents an estimate of the number of paragraphs in the document. |
| [getRevisionNumber()](#getRevisionNumber--) | Gets or sets the document revision number. |
| [getScaleCrop()](#getScaleCrop--) | Indicates the display mode of the document thumbnail. |
| [getSubject()](#getSubject--) | Gets or sets the subject of the document. |
| [getTemplate()](#getTemplate--) | Gets or sets the informational name of the document template. |
| [getTitle()](#getTitle--) | Gets or sets the title of the document. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Gets or sets the total editing time in minutes. |
| [getVersion()](#getVersion--) | Represents the version number of the application that created the document. |
| [getWords()](#getWords--) | Represents an estimate of the number of words in the document. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Gets the index of a property by name. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Removes a property with the specified name from the collection. |
| [removeAt(int index)](#removeAt-int-) | Removes a property at the specified index. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | For the description of this property, please see [getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) |
| [setBytes(int value)](#setBytes-int-) | For the description of this property, please see [getBytes()](../../com.aspose.cells/builtindocumentpropertycollection\#getBytes--) |
| [setCategory(String value)](#setCategory-java.lang.String-) | For the description of this property, please see [getCategory()](../../com.aspose.cells/builtindocumentpropertycollection\#getCategory--) |
| [setCharacters(int value)](#setCharacters-int-) | For the description of this property, please see [getCharacters()](../../com.aspose.cells/builtindocumentpropertycollection\#getCharacters--) |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | For the description of this property, please see [getCharactersWithSpaces()](../../com.aspose.cells/builtindocumentpropertycollection\#getCharactersWithSpaces--) |
| [setComments(String value)](#setComments-java.lang.String-) | For the description of this property, please see [getComments()](../../com.aspose.cells/builtindocumentpropertycollection\#getComments--) |
| [setCompany(String value)](#setCompany-java.lang.String-) | For the description of this property, please see [getCompany()](../../com.aspose.cells/builtindocumentpropertycollection\#getCompany--) |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | For the description of this property, please see [getContentStatus()](../../com.aspose.cells/builtindocumentpropertycollection\#getContentStatus--) |
| [setContentType(String value)](#setContentType-java.lang.String-) | For the description of this property, please see [getContentType()](../../com.aspose.cells/builtindocumentpropertycollection\#getContentType--) |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | For the description of this property, please see [getCreatedTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getCreatedTime--) |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | For the description of this property, please see [getCreatedUniversalTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getCreatedUniversalTime--) |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | For the description of this property, please see [getDocumentVersion()](../../com.aspose.cells/builtindocumentpropertycollection\#getDocumentVersion--) |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | For the description of this property, please see [getHyperlinkBase()](../../com.aspose.cells/builtindocumentpropertycollection\#getHyperlinkBase--) |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | For the description of this property, please see [getKeywords()](../../com.aspose.cells/builtindocumentpropertycollection\#getKeywords--) |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | For the description of this property, please see [getLanguage()](../../com.aspose.cells/builtindocumentpropertycollection\#getLanguage--) |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | For the description of this property, please see [getLastPrinted()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastPrinted--) |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | For the description of this property, please see [getLastPrintedUniversalTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastPrintedUniversalTime--) |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | For the description of this property, please see [getLastSavedBy()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastSavedBy--) |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | For the description of this property, please see [getLastSavedTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastSavedTime--) |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | For the description of this property, please see [getLastSavedUniversalTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastSavedUniversalTime--) |
| [setLines(int value)](#setLines-int-) | For the description of this property, please see [getLines()](../../com.aspose.cells/builtindocumentpropertycollection\#getLines--) |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | For the description of this property, please see [getLinksUpToDate()](../../com.aspose.cells/builtindocumentpropertycollection\#getLinksUpToDate--) |
| [setManager(String value)](#setManager-java.lang.String-) | For the description of this property, please see [getManager()](../../com.aspose.cells/builtindocumentpropertycollection\#getManager--) |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | For the description of this property, please see [getNameOfApplication()](../../com.aspose.cells/builtindocumentpropertycollection\#getNameOfApplication--) |
| [setPages(int value)](#setPages-int-) | For the description of this property, please see [getPages()](../../com.aspose.cells/builtindocumentpropertycollection\#getPages--) |
| [setParagraphs(int value)](#setParagraphs-int-) | For the description of this property, please see [getParagraphs()](../../com.aspose.cells/builtindocumentpropertycollection\#getParagraphs--) |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | For the description of this property, please see [getRevisionNumber()](../../com.aspose.cells/builtindocumentpropertycollection\#getRevisionNumber--) |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | For the description of this property, please see [getScaleCrop()](../../com.aspose.cells/builtindocumentpropertycollection\#getScaleCrop--) |
| [setSubject(String value)](#setSubject-java.lang.String-) | For the description of this property, please see [getSubject()](../../com.aspose.cells/builtindocumentpropertycollection\#getSubject--) |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | For the description of this property, please see [getTemplate()](../../com.aspose.cells/builtindocumentpropertycollection\#getTemplate--) |
| [setTitle(String value)](#setTitle-java.lang.String-) | For the description of this property, please see [getTitle()](../../com.aspose.cells/builtindocumentpropertycollection\#getTitle--) |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | For the description of this property, please see [getTotalEditingTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getTotalEditingTime--) |
| [setVersion(String value)](#setVersion-java.lang.String-) | For the description of this property, please see [getVersion()](../../com.aspose.cells/builtindocumentpropertycollection\#getVersion--) |
| [setWords(int value)](#setWords-int-) | For the description of this property, please see [getWords()](../../com.aspose.cells/builtindocumentpropertycollection\#getWords--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BuiltInDocumentPropertyCollection() {#BuiltInDocumentPropertyCollection--}
```
public BuiltInDocumentPropertyCollection()
```


### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Adds an item to the CollectionBase instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |

**Returns:**
int - The position into which the new element was inserted.
### clear() {#clear--}
```
public void clear()
```


Removes all objects from the CollectionBase instance.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Return whether instance contains this object

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |

**Returns:**
boolean - Whether instance contains this object
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Returns true if a property with the specified name exists in the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |

**Returns:**
boolean - True if the property exists in the collection; false otherwise.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Zero-based index of the [DocumentProperty](../../com.aspose.cells/documentproperty) to retrieve. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by the name of the property.

The string names of the properties correspond to the names of the typed properties available from .

If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new  is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).

If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property to retrieve. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Gets or sets the name of the document's author.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Represents an estimate of the number of bytes in the document.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Gets or sets the category of the document.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Represents an estimate of the number of characters in the document.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Represents an estimate of the number of characters (including spaces) in the document.

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


Gets or sets the document comments.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Gets or sets the company property.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Gets or sets the content status of the document.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Gets or sets the content type of the document.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Gets the number of elements contained in the CollectionBase instance.

**Returns:**
int - The number of elements contained in the CollectionBase instance.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Gets or sets date of the document creation in local timezone.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Gets or sets the Universal time of the document creation.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Represents the version of the file.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Gets or sets the hyperlinkbase property.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Gets or sets the document keywords.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Gets or sets the document's language.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Gets or sets the date when the document was last printed in local timezone.

If the document was never printed, this property will return DateTime.MinValue.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Gets or sets the Universal time when the document was last printed.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Gets or sets the name of the last author.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Gets or sets the time of the last save in local timezone.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Gets or sets the universal time of the last save.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Represents an estimate of the number of lines in the document.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Indicates whether hyperlinks in a document are up-to-date.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Gets or sets the manager property.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Gets or sets the name of the application.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Represents an estimate of the number of pages in the document.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Represents an estimate of the number of paragraphs in the document.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Gets or sets the document revision number.

Aspose.Cells does not update this property when you modify the document.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Indicates the display mode of the document thumbnail.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Gets or sets the subject of the document.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Gets or sets the informational name of the document template.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Gets or sets the title of the document.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Gets or sets the total editing time in minutes.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Represents an estimate of the number of words in the document.

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


Determines the index of a specific item in the CollectionBase instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |

**Returns:**
int - The index of value if found in the list; otherwise, -1.
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Gets the index of a property by name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |

**Returns:**
int - The zero based index. Negative value if not found.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returns an enumerator that iterates through the CollectionBase instance.

**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
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


Removes a property with the specified name from the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Removes a property at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


For the description of this property, please see [getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


For the description of this property, please see [getBytes()](../../com.aspose.cells/builtindocumentpropertycollection\#getBytes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


For the description of this property, please see [getCategory()](../../com.aspose.cells/builtindocumentpropertycollection\#getCategory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


For the description of this property, please see [getCharacters()](../../com.aspose.cells/builtindocumentpropertycollection\#getCharacters--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


For the description of this property, please see [getCharactersWithSpaces()](../../com.aspose.cells/builtindocumentpropertycollection\#getCharactersWithSpaces--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


For the description of this property, please see [getComments()](../../com.aspose.cells/builtindocumentpropertycollection\#getComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


For the description of this property, please see [getCompany()](../../com.aspose.cells/builtindocumentpropertycollection\#getCompany--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


For the description of this property, please see [getContentStatus()](../../com.aspose.cells/builtindocumentpropertycollection\#getContentStatus--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


For the description of this property, please see [getContentType()](../../com.aspose.cells/builtindocumentpropertycollection\#getContentType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


For the description of this property, please see [getCreatedTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getCreatedTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


For the description of this property, please see [getCreatedUniversalTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getCreatedUniversalTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


For the description of this property, please see [getDocumentVersion()](../../com.aspose.cells/builtindocumentpropertycollection\#getDocumentVersion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


For the description of this property, please see [getHyperlinkBase()](../../com.aspose.cells/builtindocumentpropertycollection\#getHyperlinkBase--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


For the description of this property, please see [getKeywords()](../../com.aspose.cells/builtindocumentpropertycollection\#getKeywords--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


For the description of this property, please see [getLanguage()](../../com.aspose.cells/builtindocumentpropertycollection\#getLanguage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


For the description of this property, please see [getLastPrinted()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastPrinted--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


For the description of this property, please see [getLastPrintedUniversalTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastPrintedUniversalTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


For the description of this property, please see [getLastSavedBy()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastSavedBy--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


For the description of this property, please see [getLastSavedTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastSavedTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


For the description of this property, please see [getLastSavedUniversalTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getLastSavedUniversalTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


For the description of this property, please see [getLines()](../../com.aspose.cells/builtindocumentpropertycollection\#getLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


For the description of this property, please see [getLinksUpToDate()](../../com.aspose.cells/builtindocumentpropertycollection\#getLinksUpToDate--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


For the description of this property, please see [getManager()](../../com.aspose.cells/builtindocumentpropertycollection\#getManager--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


For the description of this property, please see [getNameOfApplication()](../../com.aspose.cells/builtindocumentpropertycollection\#getNameOfApplication--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


For the description of this property, please see [getPages()](../../com.aspose.cells/builtindocumentpropertycollection\#getPages--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


For the description of this property, please see [getParagraphs()](../../com.aspose.cells/builtindocumentpropertycollection\#getParagraphs--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


For the description of this property, please see [getRevisionNumber()](../../com.aspose.cells/builtindocumentpropertycollection\#getRevisionNumber--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


For the description of this property, please see [getScaleCrop()](../../com.aspose.cells/builtindocumentpropertycollection\#getScaleCrop--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


For the description of this property, please see [getSubject()](../../com.aspose.cells/builtindocumentpropertycollection\#getSubject--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


For the description of this property, please see [getTemplate()](../../com.aspose.cells/builtindocumentpropertycollection\#getTemplate--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


For the description of this property, please see [getTitle()](../../com.aspose.cells/builtindocumentpropertycollection\#getTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


For the description of this property, please see [getTotalEditingTime()](../../com.aspose.cells/builtindocumentpropertycollection\#getTotalEditingTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


For the description of this property, please see [getVersion()](../../com.aspose.cells/builtindocumentpropertycollection\#getVersion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


For the description of this property, please see [getWords()](../../com.aspose.cells/builtindocumentpropertycollection\#getWords--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

