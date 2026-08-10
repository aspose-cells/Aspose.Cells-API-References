---
title: "BuiltInDocumentPropertyCollection"
linktitle: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "A collection of built-in document properties."
type: docs
weight: 270
url: /nodejs/aspose.cells/builtindocumentpropertycollection/
---

## BuiltInDocumentPropertyCollection class

A collection of built-in document properties. Provides access to DocumentProperty objects by their names (using an indexer) and via a set of typed properties that return values of appropriate types.

## Methods

| Name | Description |
| --- | --- |
| [add()](#add) | Reserved for internal use. |
| [clear()](#clear) |  |
| [contains(name)](#contains) | Returns true if a property with the specified name exists in the collection. |
| [contains()](#contains-1) | Reserved for internal use. |
| [get(name)](#get) | Returns a DocumentProperty object by the name of the property. The string names of the properties correspond to the name |
| [get(index)](#get-1) | Returns a DocumentProperty object by index. |
| [get()](#get-2) | Reserved for internal use. |
| [getAuthor()](#getauthor) | Gets or sets the name of the document's author. |
| [getBytes()](#getbytes) | Represents an estimate of the number of bytes in the document. |
| [getCategory()](#getcategory) | Gets or sets the category of the document. |
| [getCharacters()](#getcharacters) | Represents an estimate of the number of characters in the document. |
| [getCharactersWithSpaces()](#getcharacterswithspaces) | Represents an estimate of the number of characters (including spaces) in the document. |
| [getComments()](#getcomments) | Gets or sets the document comments. |
| [getCompany()](#getcompany) | Gets or sets the company property. |
| [getContentStatus()](#getcontentstatus) | Gets or sets the content status of the document. |
| [getContentType()](#getcontenttype) | Gets or sets the content type of the document. |
| [getCount()](#getcount) |  |
| [getCreatedTime()](#getcreatedtime) | Gets or sets date of the document creation in local timezone. Aspose.Cells does not update this property when you modify |
| [getCreatedUniversalTime()](#getcreateduniversaltime) | Gets or sets the Universal time of the document creation. Aspose.Cells does not update this property when you modify the |
| [getDocumentVersion()](#getdocumentversion) | Represents the version of the file. |
| [getHyperlinkBase()](#gethyperlinkbase) | Gets or sets the hyperlinkbase property. |
| [getKeywords()](#getkeywords) | Gets or sets the document keywords. |
| [getLanguage()](#getlanguage) | Gets or sets the document's language. |
| [getLastPrinted()](#getlastprinted) | Gets or sets the date when the document was last printed in local timezone. If the document was never printed, this prop |
| [getLastPrintedUniversalTime()](#getlastprinteduniversaltime) | Gets or sets the Universal time when the document was last printed. |
| [getLastSavedBy()](#getlastsavedby) | Gets or sets the name of the last author. Aspose.Cells does not update this property when you modify the document. |
| [getLastSavedTime()](#getlastsavedtime) | Gets or sets the time of the last save in local timezone. Aspose.Cells does not update this property when you modify the |
| [getLastSavedUniversalTime()](#getlastsaveduniversaltime) | Gets or sets the universal time of the last save. Aspose.Cells does not update this property when you modify the documen |
| [getLines()](#getlines) | Represents an estimate of the number of lines in the document. Aspose.Cells does not update this property when you modif |
| [getLinksUpToDate()](#getlinksuptodate) | Indicates whether hyperlinks in a document are up-to-date. |
| [getManager()](#getmanager) | Gets or sets the manager property. |
| [getNameOfApplication()](#getnameofapplication) | Gets or sets the name of the application. |
| [getPages()](#getpages) | Represents an estimate of the number of pages in the document. |
| [getParagraphs()](#getparagraphs) | Represents an estimate of the number of paragraphs in the document. |
| [getRevisionNumber()](#getrevisionnumber) | Gets or sets the document revision number. Aspose.Cells does not update this property when you modify the document. |
| [getScaleCrop()](#getscalecrop) | Indicates the display mode of the document thumbnail. |
| [getSubject()](#getsubject) | Gets or sets the subject of the document. |
| [getTemplate()](#gettemplate) | Gets or sets the informational name of the document template. |
| [getTitle()](#gettitle) | Gets or sets the title of the document. |
| [getTotalEditingTime()](#gettotaleditingtime) | Gets or sets the total editing time in minutes. |
| [getVersion()](#getversion) | Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.00 |
| [getWords()](#getwords) | Represents an estimate of the number of words in the document. |
| [indexOf(name)](#indexof) | Gets the index of a property by name. |
| [indexOf()](#indexof-1) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(name)](#remove) | Removes a property with the specified name from the collection. |
| [removeAt(index)](#removeat) | Removes a property at the specified index. |
| [setAuthor()](#setauthor) | Gets or sets the name of the document's author. |
| [setBytes()](#setbytes) | Represents an estimate of the number of bytes in the document. |
| [setCategory()](#setcategory) | Gets or sets the category of the document. |
| [setCharacters()](#setcharacters) | Represents an estimate of the number of characters in the document. |
| [setCharactersWithSpaces()](#setcharacterswithspaces) | Represents an estimate of the number of characters (including spaces) in the document. |
| [setComments()](#setcomments) | Gets or sets the document comments. |
| [setCompany()](#setcompany) | Gets or sets the company property. |
| [setContentStatus()](#setcontentstatus) | Gets or sets the content status of the document. |
| [setContentType()](#setcontenttype) | Gets or sets the content type of the document. |
| [setCreatedTime()](#setcreatedtime) | Gets or sets date of the document creation in local timezone. Aspose.Cells does not update this property when you modify |
| [setCreatedUniversalTime()](#setcreateduniversaltime) | Gets or sets the Universal time of the document creation. Aspose.Cells does not update this property when you modify the |
| [setDocumentVersion()](#setdocumentversion) | Represents the version of the file. |
| [setHyperlinkBase()](#sethyperlinkbase) | Gets or sets the hyperlinkbase property. |
| [setKeywords()](#setkeywords) | Gets or sets the document keywords. |
| [setLanguage()](#setlanguage) | Gets or sets the document's language. |
| [setLastPrinted()](#setlastprinted) | Gets or sets the date when the document was last printed in local timezone. If the document was never printed, this prop |
| [setLastPrintedUniversalTime()](#setlastprinteduniversaltime) | Gets or sets the Universal time when the document was last printed. |
| [setLastSavedBy()](#setlastsavedby) | Gets or sets the name of the last author. Aspose.Cells does not update this property when you modify the document. |
| [setLastSavedTime()](#setlastsavedtime) | Gets or sets the time of the last save in local timezone. Aspose.Cells does not update this property when you modify the |
| [setLastSavedUniversalTime()](#setlastsaveduniversaltime) | Gets or sets the universal time of the last save. Aspose.Cells does not update this property when you modify the documen |
| [setLines()](#setlines) | Represents an estimate of the number of lines in the document. Aspose.Cells does not update this property when you modif |
| [setLinksUpToDate()](#setlinksuptodate) | Indicates whether hyperlinks in a document are up-to-date. |
| [setManager()](#setmanager) | Gets or sets the manager property. |
| [setNameOfApplication()](#setnameofapplication) | Gets or sets the name of the application. |
| [setPages()](#setpages) | Represents an estimate of the number of pages in the document. |
| [setParagraphs()](#setparagraphs) | Represents an estimate of the number of paragraphs in the document. |
| [setRevisionNumber()](#setrevisionnumber) | Gets or sets the document revision number. Aspose.Cells does not update this property when you modify the document. |
| [setScaleCrop()](#setscalecrop) | Indicates the display mode of the document thumbnail. |
| [setSubject()](#setsubject) | Gets or sets the subject of the document. |
| [setTemplate()](#settemplate) | Gets or sets the informational name of the document template. |
| [setTitle()](#settitle) | Gets or sets the title of the document. |
| [setTotalEditingTime()](#settotaleditingtime) | Gets or sets the total editing time in minutes. |
| [setVersion()](#setversion) | Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.00 |
| [setWords()](#setwords) | Represents an estimate of the number of words in the document. |

### add() {#add}

Reserved for internal use.

### clear() {#clear}

### contains(name) {#contains}

Returns true if a property with the specified name exists in the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** boolean — `boolean` True if the property exists in the collection; false otherwise.

### contains() {#contains-1}

Reserved for internal use.

### get(name) {#get}

Returns a DocumentProperty object by the name of the property. The string names of the properties correspond to the names of the typed properties available from BuiltInDocumentPropertyCollection.If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new DocumentProperty is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property to retrieve. |

### get(index) {#get-1}

Returns a DocumentProperty object by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Zero-based index of the |

### get() {#get-2}

Reserved for internal use.

### getAuthor() {#getauthor}

Gets or sets the name of the document's author.

### getBytes() {#getbytes}

Represents an estimate of the number of bytes in the document.

### getCategory() {#getcategory}

Gets or sets the category of the document.

### getCharacters() {#getcharacters}

Represents an estimate of the number of characters in the document.

### getCharactersWithSpaces() {#getcharacterswithspaces}

Represents an estimate of the number of characters (including spaces) in the document.

### getComments() {#getcomments}

Gets or sets the document comments.

### getCompany() {#getcompany}

Gets or sets the company property.

### getContentStatus() {#getcontentstatus}

Gets or sets the content status of the document.

### getContentType() {#getcontenttype}

Gets or sets the content type of the document.

### getCount() {#getcount}

### getCreatedTime() {#getcreatedtime}

Gets or sets date of the document creation in local timezone. Aspose.Cells does not update this property when you modify the document.

### getCreatedUniversalTime() {#getcreateduniversaltime}

Gets or sets the Universal time of the document creation. Aspose.Cells does not update this property when you modify the document.

### getDocumentVersion() {#getdocumentversion}

Represents the version of the file.

### getHyperlinkBase() {#gethyperlinkbase}

Gets or sets the hyperlinkbase property.

### getKeywords() {#getkeywords}

Gets or sets the document keywords.

### getLanguage() {#getlanguage}

Gets or sets the document's language.

### getLastPrinted() {#getlastprinted}

Gets or sets the date when the document was last printed in local timezone. If the document was never printed, this property will return DateTime.MinValue.Aspose.Cells does not update this property when you modify the document.

### getLastPrintedUniversalTime() {#getlastprinteduniversaltime}

Gets or sets the Universal time when the document was last printed.

### getLastSavedBy() {#getlastsavedby}

Gets or sets the name of the last author. Aspose.Cells does not update this property when you modify the document.

### getLastSavedTime() {#getlastsavedtime}

Gets or sets the time of the last save in local timezone. Aspose.Cells does not update this property when you modify the document.

### getLastSavedUniversalTime() {#getlastsaveduniversaltime}

Gets or sets the universal time of the last save. Aspose.Cells does not update this property when you modify the document.

### getLines() {#getlines}

Represents an estimate of the number of lines in the document. Aspose.Cells does not update this property when you modify the document.

### getLinksUpToDate() {#getlinksuptodate}

Indicates whether hyperlinks in a document are up-to-date.

### getManager() {#getmanager}

Gets or sets the manager property.

### getNameOfApplication() {#getnameofapplication}

Gets or sets the name of the application.

### getPages() {#getpages}

Represents an estimate of the number of pages in the document.

### getParagraphs() {#getparagraphs}

Represents an estimate of the number of paragraphs in the document.

### getRevisionNumber() {#getrevisionnumber}

Gets or sets the document revision number. Aspose.Cells does not update this property when you modify the document.

### getScaleCrop() {#getscalecrop}

Indicates the display mode of the document thumbnail.

### getSubject() {#getsubject}

Gets or sets the subject of the document.

### getTemplate() {#gettemplate}

Gets or sets the informational name of the document template.

### getTitle() {#gettitle}

Gets or sets the title of the document.

### getTotalEditingTime() {#gettotaleditingtime}

Gets or sets the total editing time in minutes.

### getVersion() {#getversion}

Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.0000

### getWords() {#getwords}

Represents an estimate of the number of words in the document.

### indexOf(name) {#indexof}

Gets the index of a property by name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** Number — `Number` The zero based index. Negative value if not found.

### indexOf() {#indexof-1}

Reserved for internal use.

### iterator() {#iterator}

### remove(name) {#remove}

Removes a property with the specified name from the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### removeAt(index) {#removeat}

Removes a property at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index. |

### setAuthor() {#setauthor}

Gets or sets the name of the document's author.

### setBytes() {#setbytes}

Represents an estimate of the number of bytes in the document.

### setCategory() {#setcategory}

Gets or sets the category of the document.

### setCharacters() {#setcharacters}

Represents an estimate of the number of characters in the document.

### setCharactersWithSpaces() {#setcharacterswithspaces}

Represents an estimate of the number of characters (including spaces) in the document.

### setComments() {#setcomments}

Gets or sets the document comments.

### setCompany() {#setcompany}

Gets or sets the company property.

### setContentStatus() {#setcontentstatus}

Gets or sets the content status of the document.

### setContentType() {#setcontenttype}

Gets or sets the content type of the document.

### setCreatedTime() {#setcreatedtime}

Gets or sets date of the document creation in local timezone. Aspose.Cells does not update this property when you modify the document.

### setCreatedUniversalTime() {#setcreateduniversaltime}

Gets or sets the Universal time of the document creation. Aspose.Cells does not update this property when you modify the document.

### setDocumentVersion() {#setdocumentversion}

Represents the version of the file.

### setHyperlinkBase() {#sethyperlinkbase}

Gets or sets the hyperlinkbase property.

### setKeywords() {#setkeywords}

Gets or sets the document keywords.

### setLanguage() {#setlanguage}

Gets or sets the document's language.

### setLastPrinted() {#setlastprinted}

Gets or sets the date when the document was last printed in local timezone. If the document was never printed, this property will return DateTime.MinValue.Aspose.Cells does not update this property when you modify the document.

### setLastPrintedUniversalTime() {#setlastprinteduniversaltime}

Gets or sets the Universal time when the document was last printed.

### setLastSavedBy() {#setlastsavedby}

Gets or sets the name of the last author. Aspose.Cells does not update this property when you modify the document.

### setLastSavedTime() {#setlastsavedtime}

Gets or sets the time of the last save in local timezone. Aspose.Cells does not update this property when you modify the document.

### setLastSavedUniversalTime() {#setlastsaveduniversaltime}

Gets or sets the universal time of the last save. Aspose.Cells does not update this property when you modify the document.

### setLines() {#setlines}

Represents an estimate of the number of lines in the document. Aspose.Cells does not update this property when you modify the document.

### setLinksUpToDate() {#setlinksuptodate}

Indicates whether hyperlinks in a document are up-to-date.

### setManager() {#setmanager}

Gets or sets the manager property.

### setNameOfApplication() {#setnameofapplication}

Gets or sets the name of the application.

### setPages() {#setpages}

Represents an estimate of the number of pages in the document.

### setParagraphs() {#setparagraphs}

Represents an estimate of the number of paragraphs in the document.

### setRevisionNumber() {#setrevisionnumber}

Gets or sets the document revision number. Aspose.Cells does not update this property when you modify the document.

### setScaleCrop() {#setscalecrop}

Indicates the display mode of the document thumbnail.

### setSubject() {#setsubject}

Gets or sets the subject of the document.

### setTemplate() {#settemplate}

Gets or sets the informational name of the document template.

### setTitle() {#settitle}

Gets or sets the title of the document.

### setTotalEditingTime() {#settotaleditingtime}

Gets or sets the total editing time in minutes.

### setVersion() {#setversion}

Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.0000

### setWords() {#setwords}

Represents an estimate of the number of words in the document.
