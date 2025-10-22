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
| Constructor | Description |
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
| [get(number)](#get-number-)| Returns a [DocumentProperty](../documentproperty/) object by index. |
| [getLanguage()](#getLanguage--)| <b>@deprecated.</b> Please use the 'language' property instead. Gets or sets the document's language. |
| [setLanguage(string)](#setLanguage-string-)| <b>@deprecated.</b> Please use the 'language' property instead. Gets or sets the document's language. |
| [getAuthor()](#getAuthor--)| <b>@deprecated.</b> Please use the 'author' property instead. Gets or sets the name of the document's author. |
| [setAuthor(string)](#setAuthor-string-)| <b>@deprecated.</b> Please use the 'author' property instead. Gets or sets the name of the document's author. |
| [getComments()](#getComments--)| <b>@deprecated.</b> Please use the 'comments' property instead. Gets or sets the document comments. |
| [setComments(string)](#setComments-string-)| <b>@deprecated.</b> Please use the 'comments' property instead. Gets or sets the document comments. |
| [getCategory()](#getCategory--)| <b>@deprecated.</b> Please use the 'category' property instead. Gets or sets the category of the document. |
| [setCategory(string)](#setCategory-string-)| <b>@deprecated.</b> Please use the 'category' property instead. Gets or sets the category of the document. |
| [getContentType()](#getContentType--)| <b>@deprecated.</b> Please use the 'contentType' property instead. Gets or sets the content type of the document. |
| [setContentType(string)](#setContentType-string-)| <b>@deprecated.</b> Please use the 'contentType' property instead. Gets or sets the content type of the document. |
| [getContentStatus()](#getContentStatus--)| <b>@deprecated.</b> Please use the 'contentStatus' property instead. Gets or sets the content status of the document. |
| [setContentStatus(string)](#setContentStatus-string-)| <b>@deprecated.</b> Please use the 'contentStatus' property instead. Gets or sets the content status of the document. |
| [getCompany()](#getCompany--)| <b>@deprecated.</b> Please use the 'company' property instead. Gets or sets the company property. |
| [setCompany(string)](#setCompany-string-)| <b>@deprecated.</b> Please use the 'company' property instead. Gets or sets the company property. |
| [getHyperlinkBase()](#getHyperlinkBase--)| <b>@deprecated.</b> Please use the 'hyperlinkBase' property instead. Gets or sets the hyperlinkbase property. |
| [setHyperlinkBase(string)](#setHyperlinkBase-string-)| <b>@deprecated.</b> Please use the 'hyperlinkBase' property instead. Gets or sets the hyperlinkbase property. |
| [getCreatedTime()](#getCreatedTime--)| <b>@deprecated.</b> Please use the 'createdTime' property instead. Gets or sets date of the document creation in local timezone. |
| [setCreatedTime(Date)](#setCreatedTime-date-)| <b>@deprecated.</b> Please use the 'createdTime' property instead. Gets or sets date of the document creation in local timezone. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--)| <b>@deprecated.</b> Please use the 'createdUniversalTime' property instead. Gets or sets the Universal time of the document creation. |
| [setCreatedUniversalTime(Date)](#setCreatedUniversalTime-date-)| <b>@deprecated.</b> Please use the 'createdUniversalTime' property instead. Gets or sets the Universal time of the document creation. |
| [getKeywords()](#getKeywords--)| <b>@deprecated.</b> Please use the 'keywords' property instead. Gets or sets the document keywords. |
| [setKeywords(string)](#setKeywords-string-)| <b>@deprecated.</b> Please use the 'keywords' property instead. Gets or sets the document keywords. |
| [getLastPrinted()](#getLastPrinted--)| <b>@deprecated.</b> Please use the 'lastPrinted' property instead. Gets or sets the date when the document was last printed in local timezone. |
| [setLastPrinted(Date)](#setLastPrinted-date-)| <b>@deprecated.</b> Please use the 'lastPrinted' property instead. Gets or sets the date when the document was last printed in local timezone. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--)| <b>@deprecated.</b> Please use the 'lastPrintedUniversalTime' property instead. Gets or sets the Universal time when the document was last printed. |
| [setLastPrintedUniversalTime(Date)](#setLastPrintedUniversalTime-date-)| <b>@deprecated.</b> Please use the 'lastPrintedUniversalTime' property instead. Gets or sets the Universal time when the document was last printed. |
| [getLastSavedBy()](#getLastSavedBy--)| <b>@deprecated.</b> Please use the 'lastSavedBy' property instead. Gets or sets the name of the last author. |
| [setLastSavedBy(string)](#setLastSavedBy-string-)| <b>@deprecated.</b> Please use the 'lastSavedBy' property instead. Gets or sets the name of the last author. |
| [getLastSavedTime()](#getLastSavedTime--)| <b>@deprecated.</b> Please use the 'lastSavedTime' property instead. Gets or sets the time of the last save in local timezone. |
| [setLastSavedTime(Date)](#setLastSavedTime-date-)| <b>@deprecated.</b> Please use the 'lastSavedTime' property instead. Gets or sets the time of the last save in local timezone. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--)| <b>@deprecated.</b> Please use the 'lastSavedUniversalTime' property instead. Gets or sets the universal time of the last save. |
| [setLastSavedUniversalTime(Date)](#setLastSavedUniversalTime-date-)| <b>@deprecated.</b> Please use the 'lastSavedUniversalTime' property instead. Gets or sets the universal time of the last save. |
| [getManager()](#getManager--)| <b>@deprecated.</b> Please use the 'manager' property instead. Gets or sets the manager property. |
| [setManager(string)](#setManager-string-)| <b>@deprecated.</b> Please use the 'manager' property instead. Gets or sets the manager property. |
| [getNameOfApplication()](#getNameOfApplication--)| <b>@deprecated.</b> Please use the 'nameOfApplication' property instead. Gets or sets the name of the application. |
| [setNameOfApplication(string)](#setNameOfApplication-string-)| <b>@deprecated.</b> Please use the 'nameOfApplication' property instead. Gets or sets the name of the application. |
| [getPages()](#getPages--)| <b>@deprecated.</b> Please use the 'pages' property instead. Represents an estimate of the number of pages in the document. |
| [setPages(number)](#setPages-number-)| <b>@deprecated.</b> Please use the 'pages' property instead. Represents an estimate of the number of pages in the document. |
| [getRevisionNumber()](#getRevisionNumber--)| <b>@deprecated.</b> Please use the 'revisionNumber' property instead. Gets or sets the document revision number. |
| [setRevisionNumber(string)](#setRevisionNumber-string-)| <b>@deprecated.</b> Please use the 'revisionNumber' property instead. Gets or sets the document revision number. |
| [getSubject()](#getSubject--)| <b>@deprecated.</b> Please use the 'subject' property instead. Gets or sets the subject of the document. |
| [setSubject(string)](#setSubject-string-)| <b>@deprecated.</b> Please use the 'subject' property instead. Gets or sets the subject of the document. |
| [getTemplate()](#getTemplate--)| <b>@deprecated.</b> Please use the 'template' property instead. Gets or sets the informational name of the document template. |
| [setTemplate(string)](#setTemplate-string-)| <b>@deprecated.</b> Please use the 'template' property instead. Gets or sets the informational name of the document template. |
| [getTitle()](#getTitle--)| <b>@deprecated.</b> Please use the 'title' property instead. Gets or sets the title of the document. |
| [setTitle(string)](#setTitle-string-)| <b>@deprecated.</b> Please use the 'title' property instead. Gets or sets the title of the document. |
| [getTotalEditingTime()](#getTotalEditingTime--)| <b>@deprecated.</b> Please use the 'totalEditingTime' property instead. Gets or sets the total editing time in minutes. |
| [setTotalEditingTime(number)](#setTotalEditingTime-number-)| <b>@deprecated.</b> Please use the 'totalEditingTime' property instead. Gets or sets the total editing time in minutes. |
| [getVersion()](#getVersion--)| <b>@deprecated.</b> Please use the 'version' property instead. Represents the version number of the application that created the document. |
| [setVersion(string)](#setVersion-string-)| <b>@deprecated.</b> Please use the 'version' property instead. Represents the version number of the application that created the document. |
| [getDocumentVersion()](#getDocumentVersion--)| <b>@deprecated.</b> Please use the 'documentVersion' property instead. Represents the version of the file. |
| [setDocumentVersion(string)](#setDocumentVersion-string-)| <b>@deprecated.</b> Please use the 'documentVersion' property instead. Represents the version of the file. |
| [getScaleCrop()](#getScaleCrop--)| <b>@deprecated.</b> Please use the 'scaleCrop' property instead. Indicates the display mode of the document thumbnail. |
| [setScaleCrop(boolean)](#setScaleCrop-boolean-)| <b>@deprecated.</b> Please use the 'scaleCrop' property instead. Indicates the display mode of the document thumbnail. |
| [getLinksUpToDate()](#getLinksUpToDate--)| <b>@deprecated.</b> Please use the 'linksUpToDate' property instead. Indicates whether hyperlinks in a document are up-to-date. |
| [setLinksUpToDate(boolean)](#setLinksUpToDate-boolean-)| <b>@deprecated.</b> Please use the 'linksUpToDate' property instead. Indicates whether hyperlinks in a document are up-to-date. |
| [getWords()](#getWords--)| <b>@deprecated.</b> Please use the 'words' property instead. Represents an estimate of the number of words in the document. |
| [setWords(number)](#setWords-number-)| <b>@deprecated.</b> Please use the 'words' property instead. Represents an estimate of the number of words in the document. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |
| [get(string)](#get-string-)| Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
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
### getLanguage() {#getLanguage--}
```javascript
getLanguage() : string;
```
### setLanguage(string) {#setLanguage-string-}
```javascript
setLanguage(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getAuthor() {#getAuthor--}
```javascript
getAuthor() : string;
```
### setAuthor(string) {#setAuthor-string-}
```javascript
setAuthor(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getComments() {#getComments--}
```javascript
getComments() : string;
```
### setComments(string) {#setComments-string-}
```javascript
setComments(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCategory() {#getCategory--}
```javascript
getCategory() : string;
```
### setCategory(string) {#setCategory-string-}
```javascript
setCategory(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getContentType() {#getContentType--}
```javascript
getContentType() : string;
```
### setContentType(string) {#setContentType-string-}
```javascript
setContentType(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getContentStatus() {#getContentStatus--}
```javascript
getContentStatus() : string;
```
### setContentStatus(string) {#setContentStatus-string-}
```javascript
setContentStatus(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCompany() {#getCompany--}
```javascript
getCompany() : string;
```
### setCompany(string) {#setCompany-string-}
```javascript
setCompany(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getHyperlinkBase() {#getHyperlinkBase--}
```javascript
getHyperlinkBase() : string;
```
### setHyperlinkBase(string) {#setHyperlinkBase-string-}
```javascript
setHyperlinkBase(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCreatedTime() {#getCreatedTime--}
```javascript
getCreatedTime() : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### setCreatedTime(Date) {#setCreatedTime-date-}
```javascript
setCreatedTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```javascript
getCreatedUniversalTime() : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### setCreatedUniversalTime(Date) {#setCreatedUniversalTime-date-}
```javascript
setCreatedUniversalTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### getKeywords() {#getKeywords--}
```javascript
getKeywords() : string;
```
### setKeywords(string) {#setKeywords-string-}
```javascript
setKeywords(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getLastPrinted() {#getLastPrinted--}
```javascript
getLastPrinted() : Date;
```
**Remarks**
If the document was never printed, this property will return DateTime.MinValue.</p> <p>Aspose.Cells does not update this property when you modify the document.
### setLastPrinted(Date) {#setLastPrinted-date-}
```javascript
setLastPrinted(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
**Remarks**
If the document was never printed, this property will return DateTime.MinValue.</p> <p>Aspose.Cells does not update this property when you modify the document.
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```javascript
getLastPrintedUniversalTime() : Date;
```
### setLastPrintedUniversalTime(Date) {#setLastPrintedUniversalTime-date-}
```javascript
setLastPrintedUniversalTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
### getLastSavedBy() {#getLastSavedBy--}
```javascript
getLastSavedBy() : string;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### setLastSavedBy(string) {#setLastSavedBy-string-}
```javascript
setLastSavedBy(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### getLastSavedTime() {#getLastSavedTime--}
```javascript
getLastSavedTime() : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### setLastSavedTime(Date) {#setLastSavedTime-date-}
```javascript
setLastSavedTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```javascript
getLastSavedUniversalTime() : Date;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### setLastSavedUniversalTime(Date) {#setLastSavedUniversalTime-date-}
```javascript
setLastSavedUniversalTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### getManager() {#getManager--}
```javascript
getManager() : string;
```
### setManager(string) {#setManager-string-}
```javascript
setManager(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getNameOfApplication() {#getNameOfApplication--}
```javascript
getNameOfApplication() : string;
```
### setNameOfApplication(string) {#setNameOfApplication-string-}
```javascript
setNameOfApplication(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getPages() {#getPages--}
```javascript
getPages() : number;
```
### setPages(number) {#setPages-number-}
```javascript
setPages(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRevisionNumber() {#getRevisionNumber--}
```javascript
getRevisionNumber() : string;
```
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### setRevisionNumber(string) {#setRevisionNumber-string-}
```javascript
setRevisionNumber(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Aspose.Cells does not update this property when you modify the document.
### getSubject() {#getSubject--}
```javascript
getSubject() : string;
```
### setSubject(string) {#setSubject-string-}
```javascript
setSubject(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTemplate() {#getTemplate--}
```javascript
getTemplate() : string;
```
### setTemplate(string) {#setTemplate-string-}
```javascript
setTemplate(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTitle() {#getTitle--}
```javascript
getTitle() : string;
```
### setTitle(string) {#setTitle-string-}
```javascript
setTitle(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTotalEditingTime() {#getTotalEditingTime--}
```javascript
getTotalEditingTime() : number;
```
### setTotalEditingTime(number) {#setTotalEditingTime-number-}
```javascript
setTotalEditingTime(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getVersion() {#getVersion--}
```javascript
getVersion() : string;
```
**Remarks**
It's format is "00.0000",for example : 12.0000
### setVersion(string) {#setVersion-string-}
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
```javascript
getDocumentVersion() : string;
```
### setDocumentVersion(string) {#setDocumentVersion-string-}
```javascript
setDocumentVersion(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getScaleCrop() {#getScaleCrop--}
```javascript
getScaleCrop() : boolean;
```
### setScaleCrop(boolean) {#setScaleCrop-boolean-}
```javascript
setScaleCrop(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getLinksUpToDate() {#getLinksUpToDate--}
```javascript
getLinksUpToDate() : boolean;
```
### setLinksUpToDate(boolean) {#setLinksUpToDate-boolean-}
```javascript
setLinksUpToDate(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getWords() {#getWords--}
```javascript
getWords() : number;
```
### setWords(number) {#setWords-number-}
```javascript
setWords(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
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
