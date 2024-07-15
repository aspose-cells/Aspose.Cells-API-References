---
title: BuiltInDocumentPropertyCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A collection of builtin document properties.
type: docs
url: /nodejs-cpp/builtindocumentpropertycollection/
---

## BuiltInDocumentPropertyCollection class

A collection of built-in document properties.

```javascript
class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection;
```

### Remarks
<p>Provides access to [DocumentProperty](../documentproperty/) objects by their names (using an indexer) and via a set of typed properties that return values of appropriate types.</p>

## Constructors

| Name | Description |
| --- | --- |
| [constructor(DocumentPropertyCollection)](#constructor-documentpropertycollection-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [get(string)](#get-string-)| Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [getLanguage()](#getLanguage--)| Gets or sets the document's language. |
| [setLanguage(string)](#setLanguage-string-)| Gets or sets the document's language. |
| [getAuthor()](#getAuthor--)| Gets or sets the name of the document's author. |
| [setAuthor(string)](#setAuthor-string-)| Gets or sets the name of the document's author. |
| [getComments()](#getComments--)| Gets or sets the document comments. |
| [setComments(string)](#setComments-string-)| Gets or sets the document comments. |
| [getCategory()](#getCategory--)| Gets or sets the category of the document. |
| [setCategory(string)](#setCategory-string-)| Gets or sets the category of the document. |
| [getContentType()](#getContentType--)| Gets or sets the content type of the document. |
| [setContentType(string)](#setContentType-string-)| Gets or sets the content type of the document. |
| [getContentStatus()](#getContentStatus--)| Gets or sets the content status of the document. |
| [setContentStatus(string)](#setContentStatus-string-)| Gets or sets the content status of the document. |
| [getCompany()](#getCompany--)| Gets or sets the company property. |
| [setCompany(string)](#setCompany-string-)| Gets or sets the company property. |
| [getHyperlinkBase()](#getHyperlinkBase--)| Gets or sets the hyperlinkbase property. |
| [setHyperlinkBase(string)](#setHyperlinkBase-string-)| Gets or sets the hyperlinkbase property. |
| [getCreatedTime()](#getCreatedTime--)| Gets or sets date of the document creation in local timezone. |
| [setCreatedTime(Date)](#setCreatedTime-date-)| Gets or sets date of the document creation in local timezone. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--)| Gets or sets the Universal time of the document creation. |
| [setCreatedUniversalTime(Date)](#setCreatedUniversalTime-date-)| Gets or sets the Universal time of the document creation. |
| [getKeywords()](#getKeywords--)| Gets or sets the document keywords. |
| [setKeywords(string)](#setKeywords-string-)| Gets or sets the document keywords. |
| [getLastPrinted()](#getLastPrinted--)| Gets or sets the date when the document was last printed in local timezone. |
| [setLastPrinted(Date)](#setLastPrinted-date-)| Gets or sets the date when the document was last printed in local timezone. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--)| Gets or sets the Universal time when the document was last printed. |
| [setLastPrintedUniversalTime(Date)](#setLastPrintedUniversalTime-date-)| Gets or sets the Universal time when the document was last printed. |
| [getLastSavedBy()](#getLastSavedBy--)| Gets or sets the name of the last author. |
| [setLastSavedBy(string)](#setLastSavedBy-string-)| Gets or sets the name of the last author. |
| [getLastSavedTime()](#getLastSavedTime--)| Gets or sets the time of the last save in local timezone. |
| [setLastSavedTime(Date)](#setLastSavedTime-date-)| Gets or sets the time of the last save in local timezone. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--)| Gets or sets the universal time of the last save. |
| [setLastSavedUniversalTime(Date)](#setLastSavedUniversalTime-date-)| Gets or sets the universal time of the last save. |
| [getManager()](#getManager--)| Gets or sets the manager property. |
| [setManager(string)](#setManager-string-)| Gets or sets the manager property. |
| [getNameOfApplication()](#getNameOfApplication--)| Gets or sets the name of the application. |
| [setNameOfApplication(string)](#setNameOfApplication-string-)| Gets or sets the name of the application. |
| [getPages()](#getPages--)| Represents an estimate of the number of pages in the document. |
| [setPages(number)](#setPages-number-)| Represents an estimate of the number of pages in the document. |
| [getRevisionNumber()](#getRevisionNumber--)| Gets or sets the document revision number. |
| [setRevisionNumber(string)](#setRevisionNumber-string-)| Gets or sets the document revision number. |
| [getSubject()](#getSubject--)| Gets or sets the subject of the document. |
| [setSubject(string)](#setSubject-string-)| Gets or sets the subject of the document. |
| [getTemplate()](#getTemplate--)| Gets or sets the informational name of the document template. |
| [setTemplate(string)](#setTemplate-string-)| Gets or sets the informational name of the document template. |
| [getTitle()](#getTitle--)| Gets or sets the title of the document. |
| [setTitle(string)](#setTitle-string-)| Gets or sets the title of the document. |
| [getTotalEditingTime()](#getTotalEditingTime--)| Gets or sets the total editing time in minutes. |
| [setTotalEditingTime(number)](#setTotalEditingTime-number-)| Gets or sets the total editing time in minutes. |
| [getVersion()](#getVersion--)| Represents the version number of the application that created the document. |
| [setVersion(string)](#setVersion-string-)| Represents the version number of the application that created the document. |
| [getDocumentVersion()](#getDocumentVersion--)| Represents the version of the file. |
| [setDocumentVersion(string)](#setDocumentVersion-string-)| Represents the version of the file. |
| [getScaleCrop()](#getScaleCrop--)| Indicates the display mode of the document thumbnail. |
| [setScaleCrop(boolean)](#setScaleCrop-boolean-)| Indicates the display mode of the document thumbnail. |
| [getLinksUpToDate()](#getLinksUpToDate--)| Indicates whether hyperlinks in a document are up-to-date. |
| [setLinksUpToDate(boolean)](#setLinksUpToDate-boolean-)| Indicates whether hyperlinks in a document are up-to-date. |
| [getWords()](#getWords--)| Represents an estimate of the number of words in the document. |
| [setWords(number)](#setWords-number-)| Represents an estimate of the number of words in the document. |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### constructor(DocumentPropertyCollection) {#constructor-documentpropertycollection-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: DocumentPropertyCollection);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | DocumentPropertyCollection | The parent object. |

### get(string) {#get-string-}

Returns a [DocumentProperty](../documentproperty/) object by the name of the property.

```javascript
get(name: string) : DocumentProperty;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property to retrieve. |

**Returns**

[DocumentProperty](../documentproperty/)

**Remarks**

<p>The string names of the properties correspond to the names of the typed properties available from [BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/).</p> <p>If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new [DocumentProperty](../documentproperty/) is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).</p> <p>If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.</p>

### getLanguage() {#getLanguage--}

Gets or sets the document's language.

```javascript
getLanguage() : string;
```


### setLanguage(string) {#setLanguage-string-}

Gets or sets the document's language.

```javascript
setLanguage(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAuthor() {#getAuthor--}

Gets or sets the name of the document's author.

```javascript
getAuthor() : string;
```


### setAuthor(string) {#setAuthor-string-}

Gets or sets the name of the document's author.

```javascript
setAuthor(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getComments() {#getComments--}

Gets or sets the document comments.

```javascript
getComments() : string;
```


### setComments(string) {#setComments-string-}

Gets or sets the document comments.

```javascript
setComments(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCategory() {#getCategory--}

Gets or sets the category of the document.

```javascript
getCategory() : string;
```


### setCategory(string) {#setCategory-string-}

Gets or sets the category of the document.

```javascript
setCategory(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getContentType() {#getContentType--}

Gets or sets the content type of the document.

```javascript
getContentType() : string;
```


### setContentType(string) {#setContentType-string-}

Gets or sets the content type of the document.

```javascript
setContentType(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getContentStatus() {#getContentStatus--}

Gets or sets the content status of the document.

```javascript
getContentStatus() : string;
```


### setContentStatus(string) {#setContentStatus-string-}

Gets or sets the content status of the document.

```javascript
setContentStatus(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCompany() {#getCompany--}

Gets or sets the company property.

```javascript
getCompany() : string;
```


### setCompany(string) {#setCompany-string-}

Gets or sets the company property.

```javascript
setCompany(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getHyperlinkBase() {#getHyperlinkBase--}

Gets or sets the hyperlinkbase property.

```javascript
getHyperlinkBase() : string;
```


### setHyperlinkBase(string) {#setHyperlinkBase-string-}

Gets or sets the hyperlinkbase property.

```javascript
setHyperlinkBase(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCreatedTime() {#getCreatedTime--}

Gets or sets date of the document creation in local timezone.

```javascript
getCreatedTime() : Date;
```


**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### setCreatedTime(Date) {#setCreatedTime-date-}

Gets or sets date of the document creation in local timezone.

```javascript
setCreatedTime(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### getCreatedUniversalTime() {#getCreatedUniversalTime--}

Gets or sets the Universal time of the document creation.

```javascript
getCreatedUniversalTime() : Date;
```


**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### setCreatedUniversalTime(Date) {#setCreatedUniversalTime-date-}

Gets or sets the Universal time of the document creation.

```javascript
setCreatedUniversalTime(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### getKeywords() {#getKeywords--}

Gets or sets the document keywords.

```javascript
getKeywords() : string;
```


### setKeywords(string) {#setKeywords-string-}

Gets or sets the document keywords.

```javascript
setKeywords(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLastPrinted() {#getLastPrinted--}

Gets or sets the date when the document was last printed in local timezone.

```javascript
getLastPrinted() : Date;
```


**Remarks**

<p>If the document was never printed, this property will return DateTime.MinValue.</p> <p>Aspose.Cells does not update this property when you modify the document.</p>

### setLastPrinted(Date) {#setLastPrinted-date-}

Gets or sets the date when the document was last printed in local timezone.

```javascript
setLastPrinted(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

**Remarks**

<p>If the document was never printed, this property will return DateTime.MinValue.</p> <p>Aspose.Cells does not update this property when you modify the document.</p>

### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}

Gets or sets the Universal time when the document was last printed.

```javascript
getLastPrintedUniversalTime() : Date;
```


### setLastPrintedUniversalTime(Date) {#setLastPrintedUniversalTime-date-}

Gets or sets the Universal time when the document was last printed.

```javascript
setLastPrintedUniversalTime(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

### getLastSavedBy() {#getLastSavedBy--}

Gets or sets the name of the last author.

```javascript
getLastSavedBy() : string;
```


**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### setLastSavedBy(string) {#setLastSavedBy-string-}

Gets or sets the name of the last author.

```javascript
setLastSavedBy(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### getLastSavedTime() {#getLastSavedTime--}

Gets or sets the time of the last save in local timezone.

```javascript
getLastSavedTime() : Date;
```


**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### setLastSavedTime(Date) {#setLastSavedTime-date-}

Gets or sets the time of the last save in local timezone.

```javascript
setLastSavedTime(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}

Gets or sets the universal time of the last save.

```javascript
getLastSavedUniversalTime() : Date;
```


**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### setLastSavedUniversalTime(Date) {#setLastSavedUniversalTime-date-}

Gets or sets the universal time of the last save.

```javascript
setLastSavedUniversalTime(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### getManager() {#getManager--}

Gets or sets the manager property.

```javascript
getManager() : string;
```


### setManager(string) {#setManager-string-}

Gets or sets the manager property.

```javascript
setManager(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getNameOfApplication() {#getNameOfApplication--}

Gets or sets the name of the application.

```javascript
getNameOfApplication() : string;
```


### setNameOfApplication(string) {#setNameOfApplication-string-}

Gets or sets the name of the application.

```javascript
setNameOfApplication(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPages() {#getPages--}

Represents an estimate of the number of pages in the document.

```javascript
getPages() : number;
```


### setPages(number) {#setPages-number-}

Represents an estimate of the number of pages in the document.

```javascript
setPages(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRevisionNumber() {#getRevisionNumber--}

Gets or sets the document revision number.

```javascript
getRevisionNumber() : string;
```


**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### setRevisionNumber(string) {#setRevisionNumber-string-}

Gets or sets the document revision number.

```javascript
setRevisionNumber(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

<p>Aspose.Cells does not update this property when you modify the document.</p>

### getSubject() {#getSubject--}

Gets or sets the subject of the document.

```javascript
getSubject() : string;
```


### setSubject(string) {#setSubject-string-}

Gets or sets the subject of the document.

```javascript
setSubject(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTemplate() {#getTemplate--}

Gets or sets the informational name of the document template.

```javascript
getTemplate() : string;
```


### setTemplate(string) {#setTemplate-string-}

Gets or sets the informational name of the document template.

```javascript
setTemplate(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTitle() {#getTitle--}

Gets or sets the title of the document.

```javascript
getTitle() : string;
```


### setTitle(string) {#setTitle-string-}

Gets or sets the title of the document.

```javascript
setTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTotalEditingTime() {#getTotalEditingTime--}

Gets or sets the total editing time in minutes.

```javascript
getTotalEditingTime() : number;
```


### setTotalEditingTime(number) {#setTotalEditingTime-number-}

Gets or sets the total editing time in minutes.

```javascript
setTotalEditingTime(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getVersion() {#getVersion--}

Represents the version number of the application that created the document.

```javascript
getVersion() : string;
```


**Remarks**

It's format is "00.0000",for example : 12.0000

### setVersion(string) {#setVersion-string-}

Represents the version number of the application that created the document.

```javascript
setVersion(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

It's format is "00.0000",for example : 12.0000

### getDocumentVersion() {#getDocumentVersion--}

Represents the version of the file.

```javascript
getDocumentVersion() : string;
```


### setDocumentVersion(string) {#setDocumentVersion-string-}

Represents the version of the file.

```javascript
setDocumentVersion(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getScaleCrop() {#getScaleCrop--}

Indicates the display mode of the document thumbnail.

```javascript
getScaleCrop() : boolean;
```


### setScaleCrop(boolean) {#setScaleCrop-boolean-}

Indicates the display mode of the document thumbnail.

```javascript
setScaleCrop(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLinksUpToDate() {#getLinksUpToDate--}

Indicates whether hyperlinks in a document are up-to-date.

```javascript
getLinksUpToDate() : boolean;
```


### setLinksUpToDate(boolean) {#setLinksUpToDate-boolean-}

Indicates whether hyperlinks in a document are up-to-date.

```javascript
setLinksUpToDate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWords() {#getWords--}

Represents an estimate of the number of words in the document.

```javascript
getWords() : number;
```


### setWords(number) {#setWords-number-}

Represents an estimate of the number of words in the document.

```javascript
setWords(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### contains(string) {#contains-string-}

Returns true if a property with the specified name exists in the collection.

```javascript
contains(name: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |

**Returns**

True if the property exists in the collection; false otherwise.

### indexOf(string) {#indexOf-string-}

Gets the index of a property by name.

```javascript
indexOf(name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |

**Returns**

The zero based index. Negative value if not found.

### remove(string) {#remove-string-}

Removes a property with the specified name from the collection.

```javascript
remove(name: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |

### removeAt(number) {#removeAt-number-}

Removes a property at the specified index.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index. |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



