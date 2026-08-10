---
title: "BuiltInDocumentPropertyCollection Class"
linktitle: "BuiltInDocumentPropertyCollection"
articleTitle: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Python via Java"
description: "A collection of built-in document properties."
type: docs
weight: 410
url: /python-java/asposecells.api/builtindocumentpropertycollection/
---

## BuiltInDocumentPropertyCollection class

A collection of built-in document properties.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Language](#language) | String | Gets or sets the document's language. |
| [Author](#author) | String | Gets or sets the name of the document's author. |
| [Bytes](#bytes) | int | Represents an estimate of the number of bytes in the document. |
| [Characters](#characters) | int | Represents an estimate of the number of characters in the document. |
| [CharactersWithSpaces](#characterswithspaces) | int | Represents an estimate of the number of characters (including spaces) in the document. |
| [Comments](#comments) | String | Gets or sets the document comments. |
| [Category](#category) | String | Gets or sets the category of the document. |
| [ContentType](#contenttype) | String | Gets or sets the content type of the document. |
| [ContentStatus](#contentstatus) | String | Gets or sets the content status of the document. |
| [Company](#company) | String | Gets or sets the company property. |
| [HyperlinkBase](#hyperlinkbase) | String | Gets or sets the hyperlinkbase property. |
| [CreatedTime](#createdtime) | DateTime | Gets or sets date of the document creation in local timezone. Aspose.Cells does not update this property when you modify |
| [CreatedUniversalTime](#createduniversaltime) | DateTime | Gets or sets the Universal time of the document creation. Aspose.Cells does not update this property when you modify the |
| [Keywords](#keywords) | String | Gets or sets the document keywords. |
| [LastPrinted](#lastprinted) | DateTime | Gets or sets the date when the document was last printed in local timezone. If the document was never printed, this prop |
| [LastPrintedUniversalTime](#lastprinteduniversaltime) | DateTime | Gets or sets the Universal time when the document was last printed. |
| [LastSavedBy](#lastsavedby) | String | Gets or sets the name of the last author. Aspose.Cells does not update this property when you modify the document. |
| [LastSavedTime](#lastsavedtime) | DateTime | Gets or sets the time of the last save in local timezone. Aspose.Cells does not update this property when you modify the |
| [LastSavedUniversalTime](#lastsaveduniversaltime) | DateTime | Gets or sets the universal time of the last save. Aspose.Cells does not update this property when you modify the documen |
| [Lines](#lines) | int | Represents an estimate of the number of lines in the document. Aspose.Cells does not update this property when you modif |
| [Manager](#manager) | String | Gets or sets the manager property. |
| [NameOfApplication](#nameofapplication) | String | Gets or sets the name of the application. |
| [Pages](#pages) | int | Represents an estimate of the number of pages in the document. |
| [Paragraphs](#paragraphs) | int | Represents an estimate of the number of paragraphs in the document. |
| [RevisionNumber](#revisionnumber) | String | Gets or sets the document revision number. Aspose.Cells does not update this property when you modify the document. |
| [Subject](#subject) | String | Gets or sets the subject of the document. |
| [Template](#template) | String | Gets or sets the informational name of the document template. |
| [Title](#title) | String | Gets or sets the title of the document. |
| [TotalEditingTime](#totaleditingtime) | float | Gets or sets the total editing time in minutes. |
| [Version](#version) | String | Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.00 |
| [DocumentVersion](#documentversion) | String | Represents the version of the file. |
| [ScaleCrop](#scalecrop) | boolean | Indicates the display mode of the document thumbnail. |
| [LinksUpToDate](#linksuptodate) | boolean | Indicates whether hyperlinks in a document are up-to-date. |
| [Words](#words) | int | Represents an estimate of the number of words in the document. |
| [Count](#count) | int |  |
| [Item (java.lang.String)](#itemjavalangstring) | DocumentProperty | Returns a DocumentProperty object by the name of the property. The string names of the properties correspond to the name |
| [Item (int)](#itemint) | DocumentProperty | Returns a DocumentProperty object by index. |

## Methods

| Name | Description |
| --- | --- |
| [contains](#contains) | Returns true if a property with the specified name exists in the collection. |
| [indexOf](#indexof) | Gets the index of a property by name. |
| [remove](#remove) | Removes a property with the specified name from the collection. |
| [removeAt](#removeat) | Removes a property at the specified index. |
| [clear](#clear) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [add](#add) | Reserved for internal use. |

### BuiltInDocumentPropertyCollection.Language property {#language}

Gets or sets the document's language.

**Type:** String

### BuiltInDocumentPropertyCollection.Author property {#author}

Gets or sets the name of the document's author.

**Type:** String

### BuiltInDocumentPropertyCollection.Bytes property {#bytes}

Represents an estimate of the number of bytes in the document.

**Type:** int

### BuiltInDocumentPropertyCollection.Characters property {#characters}

Represents an estimate of the number of characters in the document.

**Type:** int

### BuiltInDocumentPropertyCollection.CharactersWithSpaces property {#characterswithspaces}

Represents an estimate of the number of characters (including spaces) in the document.

**Type:** int

### BuiltInDocumentPropertyCollection.Comments property {#comments}

Gets or sets the document comments.

**Type:** String

### BuiltInDocumentPropertyCollection.Category property {#category}

Gets or sets the category of the document.

**Type:** String

### BuiltInDocumentPropertyCollection.ContentType property {#contenttype}

Gets or sets the content type of the document.

**Type:** String

### BuiltInDocumentPropertyCollection.ContentStatus property {#contentstatus}

Gets or sets the content status of the document.

**Type:** String

### BuiltInDocumentPropertyCollection.Company property {#company}

Gets or sets the company property.

**Type:** String

### BuiltInDocumentPropertyCollection.HyperlinkBase property {#hyperlinkbase}

Gets or sets the hyperlinkbase property.

**Type:** String

### BuiltInDocumentPropertyCollection.CreatedTime property {#createdtime}

Gets or sets date of the document creation in local timezone. Aspose.Cells does not update this property when you modify the document.

**Type:** DateTime

### BuiltInDocumentPropertyCollection.CreatedUniversalTime property {#createduniversaltime}

Gets or sets the Universal time of the document creation. Aspose.Cells does not update this property when you modify the document.

**Type:** DateTime

### BuiltInDocumentPropertyCollection.Keywords property {#keywords}

Gets or sets the document keywords.

**Type:** String

### BuiltInDocumentPropertyCollection.LastPrinted property {#lastprinted}

Gets or sets the date when the document was last printed in local timezone. If the document was never printed, this property will return DateTime.MinValue. Aspose.Cells does not update this property when you modify the document.

**Type:** DateTime

### BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property {#lastprinteduniversaltime}

Gets or sets the Universal time when the document was last printed.

**Type:** DateTime

### BuiltInDocumentPropertyCollection.LastSavedBy property {#lastsavedby}

Gets or sets the name of the last author. Aspose.Cells does not update this property when you modify the document.

**Type:** String

### BuiltInDocumentPropertyCollection.LastSavedTime property {#lastsavedtime}

Gets or sets the time of the last save in local timezone. Aspose.Cells does not update this property when you modify the document.

**Type:** DateTime

### BuiltInDocumentPropertyCollection.LastSavedUniversalTime property {#lastsaveduniversaltime}

Gets or sets the universal time of the last save. Aspose.Cells does not update this property when you modify the document.

**Type:** DateTime

### BuiltInDocumentPropertyCollection.Lines property {#lines}

Represents an estimate of the number of lines in the document. Aspose.Cells does not update this property when you modify the document.

**Type:** int

### BuiltInDocumentPropertyCollection.Manager property {#manager}

Gets or sets the manager property.

**Type:** String

### BuiltInDocumentPropertyCollection.NameOfApplication property {#nameofapplication}

Gets or sets the name of the application.

**Type:** String

### BuiltInDocumentPropertyCollection.Pages property {#pages}

Represents an estimate of the number of pages in the document.

**Type:** int

### BuiltInDocumentPropertyCollection.Paragraphs property {#paragraphs}

Represents an estimate of the number of paragraphs in the document.

**Type:** int

### BuiltInDocumentPropertyCollection.RevisionNumber property {#revisionnumber}

Gets or sets the document revision number. Aspose.Cells does not update this property when you modify the document.

**Type:** String

### BuiltInDocumentPropertyCollection.Subject property {#subject}

Gets or sets the subject of the document.

**Type:** String

### BuiltInDocumentPropertyCollection.Template property {#template}

Gets or sets the informational name of the document template.

**Type:** String

### BuiltInDocumentPropertyCollection.Title property {#title}

Gets or sets the title of the document.

**Type:** String

### BuiltInDocumentPropertyCollection.TotalEditingTime property {#totaleditingtime}

Gets or sets the total editing time in minutes.

**Type:** float

### BuiltInDocumentPropertyCollection.Version property {#version}

Represents the version number of the application that created the document. It's format is "00.0000",for example : 12.0000

**Type:** String

### BuiltInDocumentPropertyCollection.DocumentVersion property {#documentversion}

Represents the version of the file.

**Type:** String

### BuiltInDocumentPropertyCollection.ScaleCrop property {#scalecrop}

Indicates the display mode of the document thumbnail.

**Type:** boolean

### BuiltInDocumentPropertyCollection.LinksUpToDate property {#linksuptodate}

Indicates whether hyperlinks in a document are up-to-date.

**Type:** boolean

### BuiltInDocumentPropertyCollection.Words property {#words}

Represents an estimate of the number of words in the document.

**Type:** int

### BuiltInDocumentPropertyCollection.Count property {#count}

**Type:** int

### BuiltInDocumentPropertyCollection.Item (java.lang.String) property {#itemjavalangstring}

Returns a DocumentProperty object by the name of the property. The string names of the properties correspond to the names of the typed properties available from BuiltInDocumentPropertyCollection . If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new DocumentProperty is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property). If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.

**Type:** DocumentProperty

### BuiltInDocumentPropertyCollection.Item (int) property {#itemint}

Returns a DocumentProperty object by index.

**Type:** DocumentProperty

### contains(name) (1 of 2) {#contains}

Returns true if a property with the specified name exists in the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** True if the property exists in the collection; false otherwise.

---

### contains(value) (2 of 2) {#contains-1}

Reserved for internal use.

### indexOf(name) (1 of 2) {#indexof}

Gets the index of a property by name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** The zero based index. Negative value if not found.

---

### indexOf(value) (2 of 2) {#indexof-1}

Reserved for internal use.

### remove(name) {#remove}

Removes a property with the specified name from the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### removeAt(index) {#removeat}

Removes a property at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index. |

### clear() {#clear}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### add(value) {#add}

Reserved for internal use.
