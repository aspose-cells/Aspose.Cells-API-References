##BuiltInDocumentPropertyCollection
A collection of builtin document properties.
## BuiltInDocumentPropertyCollection class
A collection of built-in document properties.
```javascript
class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection;
```
### Remarks
Provides access to [DocumentProperty](../documentproperty/) objects by their names (using an indexer) and via a set of typed properties that return values of appropriate types.
## Constructors
| Name | Description |
| --- | --- |
| [constructor(DocumentPropertyCollection)](#constructor-documentpropertycollection-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [language](#language--)| string | Gets or sets the document's language. |
| [author](#author--)| string | Gets or sets the name of the document's author. |
| [comments](#comments--)| string | Gets or sets the document comments. |
| [category](#category--)| string | Gets or sets the category of the document. |
| [contentType](#contentType--)| string | Gets or sets the content type of the document. |
| [contentStatus](#contentStatus--)| string | Gets or sets the content status of the document. |
| [company](#company--)| string | Gets or sets the company property. |
| [hyperlinkBase](#hyperlinkBase--)| string | Gets or sets the hyperlinkbase property. |
| [createdTime](#createdTime--)| Date | Gets or sets date of the document creation in local timezone. |
| [createdUniversalTime](#createdUniversalTime--)| Date | Gets or sets the Universal time of the document creation. |
| [keywords](#keywords--)| string | Gets or sets the document keywords. |
| [lastPrinted](#lastPrinted--)| Date | Gets or sets the date when the document was last printed in local timezone. |
| [lastPrintedUniversalTime](#lastPrintedUniversalTime--)| Date | Gets or sets the Universal time when the document was last printed. |
| [lastSavedBy](#lastSavedBy--)| string | Gets or sets the name of the last author. |
| [lastSavedTime](#lastSavedTime--)| Date | Gets or sets the time of the last save in local timezone. |
| [lastSavedUniversalTime](#lastSavedUniversalTime--)| Date | Gets or sets the universal time of the last save. |
| [manager](#manager--)| string | Gets or sets the manager property. |
| [nameOfApplication](#nameOfApplication--)| string | Gets or sets the name of the application. |
| [pages](#pages--)| number | Represents an estimate of the number of pages in the document. |
| [revisionNumber](#revisionNumber--)| string | Gets or sets the document revision number. |
| [subject](#subject--)| string | Gets or sets the subject of the document. |
| [template](#template--)| string | Gets or sets the informational name of the document template. |
| [title](#title--)| string | Gets or sets the title of the document. |
| [totalEditingTime](#totalEditingTime--)| number | Gets or sets the total editing time in minutes. |
| [version](#version--)| string | Represents the version number of the application that created the document. |
| [documentVersion](#documentVersion--)| string | Represents the version of the file. |
| [scaleCrop](#scaleCrop--)| boolean | Indicates the display mode of the document thumbnail. |
| [linksUpToDate](#linksUpToDate--)| boolean | Indicates whether hyperlinks in a document are up-to-date. |
| [words](#words--)| number | Represents an estimate of the number of words in the document. |
## Methods
| Method | Description |
| --- | --- |
| [get(string)](#get-string-)| Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [get(number)](#get-number-)| Returns a [DocumentProperty](../documentproperty/) object by index. |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |
### constructor(DocumentPropertyCollection) {#constructor-documentpropertycollection-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: DocumentPropertyCollection);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | DocumentPropertyCollection | The parent object. |
### language {#language--}
Gets or sets the document's language.
```javascript
language : string;
```
### author {#author--}
Gets or sets the name of the document's author.
```javascript
author : string;
```
### comments {#comments--}
Gets or sets the document comments.
```javascript
comments : string;
```
### category {#category--}
Gets or sets the category of the document.
```javascript
category : string;
```
### contentType {#contentType--}
Gets or sets the content type of the document.
```javascript
contentType : string;
```
### contentStatus {#contentStatus--}
Gets or sets the content status of the document.
```javascript
contentStatus : string;
```
### company {#company--}
Gets or sets the company property.
```javascript
company : string;
```
### hyperlinkBase {#hyperlinkBase--}
Gets or sets the hyperlinkbase property.
```javascript
hyperlinkBase : string;
```
### createdTime {#createdTime--}
Gets or sets date of the document creation in local timezone.
```javascript
createdTime : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### createdUniversalTime {#createdUniversalTime--}
Gets or sets the Universal time of the document creation.
```javascript
createdUniversalTime : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### keywords {#keywords--}
Gets or sets the document keywords.
```javascript
keywords : string;
```
### lastPrinted {#lastPrinted--}
Gets or sets the date when the document was last printed in local timezone.
```javascript
lastPrinted : Date;
```
**Remarks**
If the document was never printed, this property will return DateTime.MinValue.</p> <p>Aspose.Cells does not update this property when you modify the document.
### lastPrintedUniversalTime {#lastPrintedUniversalTime--}
Gets or sets the Universal time when the document was last printed.
```javascript
lastPrintedUniversalTime : Date;
```
### lastSavedBy {#lastSavedBy--}
Gets or sets the name of the last author.
```javascript
lastSavedBy : string;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### lastSavedTime {#lastSavedTime--}
Gets or sets the time of the last save in local timezone.
```javascript
lastSavedTime : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### lastSavedUniversalTime {#lastSavedUniversalTime--}
Gets or sets the universal time of the last save.
```javascript
lastSavedUniversalTime : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### manager {#manager--}
Gets or sets the manager property.
```javascript
manager : string;
```
### nameOfApplication {#nameOfApplication--}
Gets or sets the name of the application.
```javascript
nameOfApplication : string;
```
### pages {#pages--}
Represents an estimate of the number of pages in the document.
```javascript
pages : number;
```
### revisionNumber {#revisionNumber--}
Gets or sets the document revision number.
```javascript
revisionNumber : string;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### subject {#subject--}
Gets or sets the subject of the document.
```javascript
subject : string;
```
### template {#template--}
Gets or sets the informational name of the document template.
```javascript
template : string;
```
### title {#title--}
Gets or sets the title of the document.
```javascript
title : string;
```
### totalEditingTime {#totalEditingTime--}
Gets or sets the total editing time in minutes.
```javascript
totalEditingTime : number;
```
### version {#version--}
Represents the version number of the application that created the document.
```javascript
version : string;
```
**Remarks**
It's format is "00.0000",for example : 12.0000
### documentVersion {#documentVersion--}
Represents the version of the file.
```javascript
documentVersion : string;
```
### scaleCrop {#scaleCrop--}
Indicates the display mode of the document thumbnail.
```javascript
scaleCrop : boolean;
```
### linksUpToDate {#linksUpToDate--}
Indicates whether hyperlinks in a document are up-to-date.
```javascript
linksUpToDate : boolean;
```
### words {#words--}
Represents an estimate of the number of words in the document.
```javascript
words : number;
```
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
The string names of the properties correspond to the names of the typed properties available from [BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/).</p> <p>If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new [DocumentProperty](../documentproperty/) is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).</p> <p>If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.
### get(number) {#get-number-}
Returns a [DocumentProperty](../documentproperty/) object by index.
```javascript
get(index: number) : DocumentProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Zero-based index of the [DocumentProperty](../documentproperty/) to retrieve. |
**Returns**
[DocumentProperty](../documentproperty/)
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
