##BuiltInDocumentPropertyCollection Class
'BuiltInDocumentPropertyCollection class. Encapsulates the object that represents builtindocumentpropertycollection in Go.'
## BuiltInDocumentPropertyCollection class
A collection of built-in document properties.
```go
type BuiltInDocumentPropertyCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewBuiltInDocumentPropertyCollection](./newbuiltindocumentpropertycollection/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Get_String](./get_string/) | Returns a DocumentProperty object by the name of the property. |
|[Get_Int](./get_int/) | Returns a DocumentProperty object by index. |
|[GetLanguage](./getlanguage/) | Gets or sets the document's language. |
|[SetLanguage](./setlanguage/) | Gets or sets the document's language. |
|[GetAuthor](./getauthor/) | Gets or sets the name of the document's author. |
|[SetAuthor](./setauthor/) | Gets or sets the name of the document's author. |
|[GetComments](./getcomments/) | Gets or sets the document comments. |
|[SetComments](./setcomments/) | Gets or sets the document comments. |
|[GetCategory](./getcategory/) | Gets or sets the category of the document. |
|[SetCategory](./setcategory/) | Gets or sets the category of the document. |
|[GetContentType](./getcontenttype/) | Gets or sets the content type of the document. |
|[SetContentType](./setcontenttype/) | Gets or sets the content type of the document. |
|[GetContentStatus](./getcontentstatus/) | Gets or sets the content status of the document. |
|[SetContentStatus](./setcontentstatus/) | Gets or sets the content status of the document. |
|[GetCompany](./getcompany/) | Gets or sets the company property. |
|[SetCompany](./setcompany/) | Gets or sets the company property. |
|[GetHyperlinkBase](./gethyperlinkbase/) | Gets or sets the hyperlinkbase property. |
|[SetHyperlinkBase](./sethyperlinkbase/) | Gets or sets the hyperlinkbase property. |
|[GetCreatedTime](./getcreatedtime/) | Gets or sets date of the document creation in local timezone. |
|[SetCreatedTime](./setcreatedtime/) | Gets or sets date of the document creation in local timezone. |
|[GetCreatedUniversalTime](./getcreateduniversaltime/) | Gets or sets the Universal time of the document creation. |
|[SetCreatedUniversalTime](./setcreateduniversaltime/) | Gets or sets the Universal time of the document creation. |
|[GetKeywords](./getkeywords/) | Gets or sets the document keywords. |
|[SetKeywords](./setkeywords/) | Gets or sets the document keywords. |
|[GetLastPrinted](./getlastprinted/) | Gets or sets the date when the document was last printed in local timezone. |
|[SetLastPrinted](./setlastprinted/) | Gets or sets the date when the document was last printed in local timezone. |
|[GetLastPrintedUniversalTime](./getlastprinteduniversaltime/) | Gets or sets the Universal time when the document was last printed. |
|[SetLastPrintedUniversalTime](./setlastprinteduniversaltime/) | Gets or sets the Universal time when the document was last printed. |
|[GetLastSavedBy](./getlastsavedby/) | Gets or sets the name of the last author. |
|[SetLastSavedBy](./setlastsavedby/) | Gets or sets the name of the last author. |
|[GetLastSavedTime](./getlastsavedtime/) | Gets or sets the time of the last save in local timezone. |
|[SetLastSavedTime](./setlastsavedtime/) | Gets or sets the time of the last save in local timezone. |
|[GetLastSavedUniversalTime](./getlastsaveduniversaltime/) | Gets or sets the universal time of the last save. |
|[SetLastSavedUniversalTime](./setlastsaveduniversaltime/) | Gets or sets the universal time of the last save. |
|[GetManager](./getmanager/) | Gets or sets the manager property. |
|[SetManager](./setmanager/) | Gets or sets the manager property. |
|[GetNameOfApplication](./getnameofapplication/) | Gets or sets the name of the application. |
|[SetNameOfApplication](./setnameofapplication/) | Gets or sets the name of the application. |
|[GetPages](./getpages/) | Represents an estimate of the number of pages in the document. |
|[SetPages](./setpages/) | Represents an estimate of the number of pages in the document. |
|[GetRevisionNumber](./getrevisionnumber/) | Gets or sets the document revision number. |
|[SetRevisionNumber](./setrevisionnumber/) | Gets or sets the document revision number. |
|[GetSubject](./getsubject/) | Gets or sets the subject of the document. |
|[SetSubject](./setsubject/) | Gets or sets the subject of the document. |
|[GetTemplate](./gettemplate/) | Gets or sets the informational name of the document template. |
|[SetTemplate](./settemplate/) | Gets or sets the informational name of the document template. |
|[GetTitle](./gettitle/) | Gets or sets the title of the document. |
|[SetTitle](./settitle/) | Gets or sets the title of the document. |
|[GetTotalEditingTime](./gettotaleditingtime/) | Gets or sets the total editing time in minutes. |
|[SetTotalEditingTime](./settotaleditingtime/) | Gets or sets the total editing time in minutes. |
|[GetVersion](./getversion/) | Represents the version number of the application that created the document. |
|[SetVersion](./setversion/) | Represents the version number of the application that created the document. |
|[GetDocumentVersion](./getdocumentversion/) | Represents the version of the file. |
|[SetDocumentVersion](./setdocumentversion/) | Represents the version of the file. |
|[GetScaleCrop](./getscalecrop/) | Indicates the display mode of the document thumbnail. |
|[SetScaleCrop](./setscalecrop/) | Indicates the display mode of the document thumbnail. |
|[GetLinksUpToDate](./getlinksuptodate/) | Indicates whether hyperlinks in a document are up-to-date. |
|[SetLinksUpToDate](./setlinksuptodate/) | Indicates whether hyperlinks in a document are up-to-date. |
|[GetWords](./getwords/) | Represents an estimate of the number of words in the document. |
|[SetWords](./setwords/) | Represents an estimate of the number of words in the document. |
|[Contains](./contains/) | Returns true if a property with the specified name exists in the collection. |
|[IndexOf](./indexof/) | Gets the index of a property by name. |
|[Remove](./remove/) | Removes a property with the specified name from the collection. |
|[RemoveAt](./removeat/) | Removes a property at the specified index. |
|[GetCount](./getcount/) |  |
