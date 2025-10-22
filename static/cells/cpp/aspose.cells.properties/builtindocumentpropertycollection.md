##Aspose::Cells::Properties::BuiltInDocumentPropertyCollection class
'Aspose::Cells::Properties::BuiltInDocumentPropertyCollection class. A collection of built-in document properties in C++.'
## BuiltInDocumentPropertyCollection class
A collection of built-in document properties.
```cpp
class BuiltInDocumentPropertyCollection : public Aspose::Cells::Properties::DocumentPropertyCollection
```
## Methods
| Method | Description |
| --- | --- |
| [BuiltInDocumentPropertyCollection(BuiltInDocumentPropertyCollection_Impl* impl)](./builtindocumentpropertycollection/) | Constructs from an implementation object. |
| [BuiltInDocumentPropertyCollection(const BuiltInDocumentPropertyCollection\& src)](./builtindocumentpropertycollection/) | Copy constructor. |
| [BuiltInDocumentPropertyCollection(const DocumentPropertyCollection\& src)](./builtindocumentpropertycollection/) | Constructs from a parent object. |
| [Contains(const U16String\& name)](../documentpropertycollection/contains/) | Returns true if a property with the specified name exists in the collection. |
| [Contains(const char16_t* name)](../documentpropertycollection/contains/) | Returns true if a property with the specified name exists in the collection. |
| [DocumentPropertyCollection(DocumentPropertyCollection_Impl* impl)](../documentpropertycollection/documentpropertycollection/) | Constructs from an implementation object. |
| [DocumentPropertyCollection(const DocumentPropertyCollection\& src)](../documentpropertycollection/documentpropertycollection/) | Copy constructor. |
| [Get(const U16String\& name)](./get/) | Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [Get(const char16_t* name)](./get/) | Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [Get(int32_t index)](./get/) | Returns a [DocumentProperty](../documentproperty/) object by index. |
| [GetAuthor()](./getauthor/) | Gets or sets the name of the document's author. |
| [GetCategory()](./getcategory/) | Gets or sets the category of the document. |
| [GetComments()](./getcomments/) | Gets or sets the document comments. |
| [GetCompany()](./getcompany/) | Gets or sets the company property. |
| [GetContentStatus()](./getcontentstatus/) | Gets or sets the content status of the document. |
| [GetContentType()](./getcontenttype/) | Gets or sets the content type of the document. |
| [GetCount()](../documentpropertycollection/getcount/) |  |
| [GetCreatedTime()](./getcreatedtime/) | Gets or sets date of the document creation in local timezone. |
| [GetCreatedUniversalTime()](./getcreateduniversaltime/) | Gets or sets the Universal time of the document creation. |
| [GetDocumentVersion()](./getdocumentversion/) | Represents the version of the file. |
| [GetHyperlinkBase()](./gethyperlinkbase/) | Gets or sets the hyperlinkbase property. |
| [GetKeywords()](./getkeywords/) | Gets or sets the document keywords. |
| [GetLanguage()](./getlanguage/) | Gets or sets the document's language. |
| [GetLastPrinted()](./getlastprinted/) | Gets or sets the date when the document was last printed in local timezone. |
| [GetLastPrintedUniversalTime()](./getlastprinteduniversaltime/) | Gets or sets the Universal time when the document was last printed. |
| [GetLastSavedBy()](./getlastsavedby/) | Gets or sets the name of the last author. |
| [GetLastSavedTime()](./getlastsavedtime/) | Gets or sets the time of the last save in local timezone. |
| [GetLastSavedUniversalTime()](./getlastsaveduniversaltime/) | Gets or sets the universal time of the last save. |
| [GetLinksUpToDate()](./getlinksuptodate/) | Indicates whether hyperlinks in a document are up-to-date. |
| [GetManager()](./getmanager/) | Gets or sets the manager property. |
| [GetNameOfApplication()](./getnameofapplication/) | Gets or sets the name of the application. |
| [GetPages()](./getpages/) | Represents an estimate of the number of pages in the document. |
| [GetRevisionNumber()](./getrevisionnumber/) | Gets or sets the document revision number. |
| [GetScaleCrop()](./getscalecrop/) | Indicates the display mode of the document thumbnail. |
| [GetSubject()](./getsubject/) | Gets or sets the subject of the document. |
| [GetTemplate()](./gettemplate/) | Gets or sets the informational name of the document template. |
| [GetTitle()](./gettitle/) | Gets or sets the title of the document. |
| [GetTotalEditingTime()](./gettotaleditingtime/) | Gets or sets the total editing time in minutes. |
| [GetVersion()](./getversion/) | Represents the version number of the application that created the document. |
| [GetWords()](./getwords/) | Represents an estimate of the number of words in the document. |
| [IndexOf(const U16String\& name)](../documentpropertycollection/indexof/) | Gets the index of a property by name. |
| [IndexOf(const char16_t* name)](../documentpropertycollection/indexof/) | Gets the index of a property by name. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const BuiltInDocumentPropertyCollection\& src)](./operator_asm/) | operator= |
| [operator=(const DocumentPropertyCollection\& src)](../documentpropertycollection/operator_asm/) | operator= |
| [Remove(const U16String\& name)](../documentpropertycollection/remove/) | Removes a property with the specified name from the collection. |
| [Remove(const char16_t* name)](../documentpropertycollection/remove/) | Removes a property with the specified name from the collection. |
| [RemoveAt(int32_t index)](../documentpropertycollection/removeat/) | Removes a property at the specified index. |
| [SetAuthor(const U16String\& value)](./setauthor/) | Gets or sets the name of the document's author. |
| [SetAuthor(const char16_t* value)](./setauthor/) | Gets or sets the name of the document's author. |
| [SetCategory(const U16String\& value)](./setcategory/) | Gets or sets the category of the document. |
| [SetCategory(const char16_t* value)](./setcategory/) | Gets or sets the category of the document. |
| [SetComments(const U16String\& value)](./setcomments/) | Gets or sets the document comments. |
| [SetComments(const char16_t* value)](./setcomments/) | Gets or sets the document comments. |
| [SetCompany(const U16String\& value)](./setcompany/) | Gets or sets the company property. |
| [SetCompany(const char16_t* value)](./setcompany/) | Gets or sets the company property. |
| [SetContentStatus(const U16String\& value)](./setcontentstatus/) | Gets or sets the content status of the document. |
| [SetContentStatus(const char16_t* value)](./setcontentstatus/) | Gets or sets the content status of the document. |
| [SetContentType(const U16String\& value)](./setcontenttype/) | Gets or sets the content type of the document. |
| [SetContentType(const char16_t* value)](./setcontenttype/) | Gets or sets the content type of the document. |
| [SetCreatedTime(const Date\& value)](./setcreatedtime/) | Gets or sets date of the document creation in local timezone. |
| [SetCreatedUniversalTime(const Date\& value)](./setcreateduniversaltime/) | Gets or sets the Universal time of the document creation. |
| [SetDocumentVersion(const U16String\& value)](./setdocumentversion/) | Represents the version of the file. |
| [SetDocumentVersion(const char16_t* value)](./setdocumentversion/) | Represents the version of the file. |
| [SetHyperlinkBase(const U16String\& value)](./sethyperlinkbase/) | Gets or sets the hyperlinkbase property. |
| [SetHyperlinkBase(const char16_t* value)](./sethyperlinkbase/) | Gets or sets the hyperlinkbase property. |
| [SetKeywords(const U16String\& value)](./setkeywords/) | Gets or sets the document keywords. |
| [SetKeywords(const char16_t* value)](./setkeywords/) | Gets or sets the document keywords. |
| [SetLanguage(const U16String\& value)](./setlanguage/) | Gets or sets the document's language. |
| [SetLanguage(const char16_t* value)](./setlanguage/) | Gets or sets the document's language. |
| [SetLastPrinted(const Date\& value)](./setlastprinted/) | Gets or sets the date when the document was last printed in local timezone. |
| [SetLastPrintedUniversalTime(const Date\& value)](./setlastprinteduniversaltime/) | Gets or sets the Universal time when the document was last printed. |
| [SetLastSavedBy(const U16String\& value)](./setlastsavedby/) | Gets or sets the name of the last author. |
| [SetLastSavedBy(const char16_t* value)](./setlastsavedby/) | Gets or sets the name of the last author. |
| [SetLastSavedTime(const Date\& value)](./setlastsavedtime/) | Gets or sets the time of the last save in local timezone. |
| [SetLastSavedUniversalTime(const Date\& value)](./setlastsaveduniversaltime/) | Gets or sets the universal time of the last save. |
| [SetLinksUpToDate(bool value)](./setlinksuptodate/) | Indicates whether hyperlinks in a document are up-to-date. |
| [SetManager(const U16String\& value)](./setmanager/) | Gets or sets the manager property. |
| [SetManager(const char16_t* value)](./setmanager/) | Gets or sets the manager property. |
| [SetNameOfApplication(const U16String\& value)](./setnameofapplication/) | Gets or sets the name of the application. |
| [SetNameOfApplication(const char16_t* value)](./setnameofapplication/) | Gets or sets the name of the application. |
| [SetPages(int32_t value)](./setpages/) | Represents an estimate of the number of pages in the document. |
| [SetRevisionNumber(const U16String\& value)](./setrevisionnumber/) | Gets or sets the document revision number. |
| [SetRevisionNumber(const char16_t* value)](./setrevisionnumber/) | Gets or sets the document revision number. |
| [SetScaleCrop(bool value)](./setscalecrop/) | Indicates the display mode of the document thumbnail. |
| [SetSubject(const U16String\& value)](./setsubject/) | Gets or sets the subject of the document. |
| [SetSubject(const char16_t* value)](./setsubject/) | Gets or sets the subject of the document. |
| [SetTemplate(const U16String\& value)](./settemplate/) | Gets or sets the informational name of the document template. |
| [SetTemplate(const char16_t* value)](./settemplate/) | Gets or sets the informational name of the document template. |
| [SetTitle(const U16String\& value)](./settitle/) | Gets or sets the title of the document. |
| [SetTitle(const char16_t* value)](./settitle/) | Gets or sets the title of the document. |
| [SetTotalEditingTime(double value)](./settotaleditingtime/) | Gets or sets the total editing time in minutes. |
| [SetVersion(const U16String\& value)](./setversion/) | Represents the version number of the application that created the document. |
| [SetVersion(const char16_t* value)](./setversion/) | Represents the version number of the application that created the document. |
| [SetWords(int32_t value)](./setwords/) | Represents an estimate of the number of words in the document. |
| [~BuiltInDocumentPropertyCollection()](./~builtindocumentpropertycollection/) | Destructor. |
| [~DocumentPropertyCollection()](../documentpropertycollection/~documentpropertycollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
Provides access to [DocumentProperty](../documentproperty/) objects by their names (using an indexer) and via a set of typed properties that return values of appropriate types.
## See Also
* Class [DocumentPropertyCollection](../documentpropertycollection/)
* Namespace [Aspose::Cells::Properties](../)
* Library [Aspose.Cells for C++](../../)
