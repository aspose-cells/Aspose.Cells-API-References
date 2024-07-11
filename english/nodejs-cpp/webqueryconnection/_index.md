---
title: WebQueryConnection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.
type: docs
url: /nodejs-cpp/webqueryconnection/
---

## WebQueryConnection class

Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.

```javascript
class WebQueryConnection extends ExternalConnection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ExternalConnection)](#constructor-externalconnection-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [isXml()](#isXml--)| true if the web query source is XML (versus HTML), otherwise false. |
| [setIsXml(boolean)](#setIsXml-boolean-)| true if the web query source is XML (versus HTML), otherwise false. |
| [isXl97()](#isXl97--)| This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored. |
| [setIsXl97(boolean)](#setIsXl97-boolean-)| This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored. |
| [isXl2000()](#isXl2000--)| This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored. |
| [setIsXl2000(boolean)](#setIsXl2000-boolean-)| This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored. |
| [getUrl()](#getUrl--)| URL to use to refresh external data. |
| [setUrl(string)](#setUrl-string-)| URL to use to refresh external data. |
| [isTextDates()](#isTextDates--)| Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [setIsTextDates(boolean)](#setIsTextDates-boolean-)| Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [isXmlSourceData()](#isXmlSourceData--)| Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [setIsXmlSourceData(boolean)](#setIsXmlSourceData-boolean-)| Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [getPost()](#getPost--)| Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| [setPost(string)](#setPost-string-)| Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| [isParsePre()](#isParsePre--)| Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table. |
| [setIsParsePre(boolean)](#setIsParsePre-boolean-)| Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table. |
| [isHtmlTables()](#isHtmlTables--)| Flag indicating whether web queries should only work on HTML tables. |
| [setIsHtmlTables(boolean)](#setIsHtmlTables-boolean-)| Flag indicating whether web queries should only work on HTML tables. |
| [getHtmlFormat()](#getHtmlFormat--)| How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True. |
| [setHtmlFormat(HtmlFormatHandlingType)](#setHtmlFormat-htmlformathandlingtype-)| How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True. |
| [isSameSettings()](#isSameSettings--)| Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [setIsSameSettings(boolean)](#setIsSameSettings-boolean-)| Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [getEditWebPage()](#getEditWebPage--)| The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [setEditWebPage(string)](#setEditWebPage-string-)| The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. |
| [isConsecutive()](#isConsecutive--)| Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [setIsConsecutive(boolean)](#setIsConsecutive-boolean-)| Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [getId()](#getId--)| Gets the id of the connection. |
| [getType()](#getType--)| Gets or Sets the external connection DataSource type. |
| [setType(ConnectionDataSourceType)](#setType-connectiondatasourcetype-)| Gets or Sets the external connection DataSource type. |
| [getSourceFile()](#getSourceFile--)| Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [setSourceFile(string)](#setSourceFile-string-)| Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation. |
| [getSSOId()](#getSSOId--)| Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [setSSOId(string)](#setSSOId-string-)| Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [getSavePassword()](#getSavePassword--)| True if the password is to be saved as part of the connection string; otherwise, False. |
| [setSavePassword(boolean)](#setSavePassword-boolean-)| True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSaveData()](#getSaveData--)| True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [setSaveData(boolean)](#setSaveData-boolean-)| True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [getRefreshOnLoad()](#getRefreshOnLoad--)| True if this connection should be refreshed when opening the file; otherwise, false. |
| [setRefreshOnLoad(boolean)](#setRefreshOnLoad-boolean-)| True if this connection should be refreshed when opening the file; otherwise, false. |
| [getReconnectionMethodType()](#getReconnectionMethodType--)| Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [setReconnectionMethodType(ReConnectionMethodType)](#setReconnectionMethodType-reconnectionmethodtype-)| Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--)| Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [setOnlyUseConnectionFile(boolean)](#setOnlyUseConnectionFile-boolean-)| Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute |
| [getOdcFile()](#getOdcFile--)| Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [setOdcFile(string)](#setOdcFile-string-)| Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook. |
| [isNew()](#isNew--)| True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [setIsNew(boolean)](#setIsNew-boolean-)| True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning. |
| [getName()](#getName--)| Specifies the name of the connection. Each connection must have a unique name. |
| [setName(string)](#setName-string-)| Specifies the name of the connection. Each connection must have a unique name. |
| [getKeepAlive()](#getKeepAlive--)| True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [setKeepAlive(boolean)](#setKeepAlive-boolean-)| True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information. |
| [getRefreshInternal()](#getRefreshInternal--)| Specifies the number of minutes between automatic refreshes of the connection. |
| [setRefreshInternal(number)](#setRefreshInternal-number-)| Specifies the number of minutes between automatic refreshes of the connection. |
| [getConnectionId()](#getConnectionId--)| Specifies The unique identifier of this connection. |
| [getConnectionDescription()](#getConnectionDescription--)| Specifies the user description for this connection |
| [setConnectionDescription(string)](#setConnectionDescription-string-)| Specifies the user description for this connection |
| [isDeleted()](#isDeleted--)| Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [setIsDeleted(boolean)](#setIsDeleted-boolean-)| Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false. |
| [getCredentialsMethodType()](#getCredentialsMethodType--)| Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [setCredentialsMethodType(CredentialsMethodType)](#setCredentialsMethodType-credentialsmethodtype-)| Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getBackgroundRefresh()](#getBackgroundRefresh--)| Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [setBackgroundRefresh(boolean)](#setBackgroundRefresh-boolean-)| Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground. |
| [getParameters()](#getParameters--)| Gets [ConnectionParameterCollection](./connectionparametercollection/) for an ODBC or web query. |
| [getPowerQueryFormula()](#getPowerQueryFormula--)| Gets the definition of power query formula. |


### constructor(ExternalConnection) {#constructor-externalconnection-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: ExternalConnection);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | ExternalConnection | The parent object. |

### isXml() {#isXml--}

true if the web query source is XML (versus HTML), otherwise false.

```javascript
isXml() : boolean;
```


### setIsXml(boolean) {#setIsXml-boolean-}

true if the web query source is XML (versus HTML), otherwise false.

```javascript
setIsXml(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isXl97() {#isXl97--}

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored.

```javascript
isXl97() : boolean;
```


### setIsXl97(boolean) {#setIsXl97-boolean-}

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored.

```javascript
setIsXl97(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isXl2000() {#isXl2000--}

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored.

```javascript
isXl2000() : boolean;
```


### setIsXl2000(boolean) {#setIsXl2000-boolean-}

This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored.

```javascript
setIsXl2000(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUrl() {#getUrl--}

URL to use to refresh external data.

```javascript
getUrl() : string;
```


### setUrl(string) {#setUrl-string-}

URL to use to refresh external data.

```javascript
setUrl(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isTextDates() {#isTextDates--}

Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates.

```javascript
isTextDates() : boolean;
```


### setIsTextDates(boolean) {#setIsTextDates-boolean-}

Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates.

```javascript
setIsTextDates(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isXmlSourceData() {#isXmlSourceData--}

Flag indicating that XML source data should be imported instead of the HTML table itself.

```javascript
isXmlSourceData() : boolean;
```


### setIsXmlSourceData(boolean) {#setIsXmlSourceData-boolean-}

Flag indicating that XML source data should be imported instead of the HTML table itself.

```javascript
setIsXmlSourceData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPost() {#getPost--}

Returns or sets the string used with the post method of inputting data into a web server to return data from a web query.

```javascript
getPost() : string;
```


### setPost(string) {#setPost-string-}

Returns or sets the string used with the post method of inputting data into a web server to return data from a web query.

```javascript
setPost(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isParsePre() {#isParsePre--}

Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table.

```javascript
isParsePre() : boolean;
```


### setIsParsePre(boolean) {#setIsParsePre-boolean-}

Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table.

```javascript
setIsParsePre(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHtmlTables() {#isHtmlTables--}

Flag indicating whether web queries should only work on HTML tables.

```javascript
isHtmlTables() : boolean;
```


### setIsHtmlTables(boolean) {#setIsHtmlTables-boolean-}

Flag indicating whether web queries should only work on HTML tables.

```javascript
setIsHtmlTables(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHtmlFormat() {#getHtmlFormat--}

How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True.

```javascript
getHtmlFormat() : HtmlFormatHandlingType;
```


**Returns**

[HtmlFormatHandlingType](./htmlformathandlingtype/)

### setHtmlFormat(HtmlFormatHandlingType) {#setHtmlFormat-htmlformathandlingtype-}

How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True.

```javascript
setHtmlFormat(value: HtmlFormatHandlingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlFormatHandlingType](./htmlformathandlingtype/) | The value to set. |

### isSameSettings() {#isSameSettings--}

Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row.

```javascript
isSameSettings() : boolean;
```


### setIsSameSettings(boolean) {#setIsSameSettings-boolean-}

Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row.

```javascript
setIsSameSettings(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEditWebPage() {#getEditWebPage--}

The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes.

```javascript
getEditWebPage() : string;
```


### setEditWebPage(string) {#setEditWebPage-string-}

The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes.

```javascript
setEditWebPage(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isConsecutive() {#isConsecutive--}

Flag indicating whether consecutive delimiters should be treated as just one delimiter.

```javascript
isConsecutive() : boolean;
```


### setIsConsecutive(boolean) {#setIsConsecutive-boolean-}

Flag indicating whether consecutive delimiters should be treated as just one delimiter.

```javascript
setIsConsecutive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getId() {#getId--}

Gets the id of the connection.

```javascript
getId() : number;
```


### getType() {#getType--}

Gets or Sets the external connection DataSource type.

```javascript
getType() : ConnectionDataSourceType;
```


**Returns**

[ConnectionDataSourceType](./connectiondatasourcetype/)

### setType(ConnectionDataSourceType) {#setType-connectiondatasourcetype-}

Gets or Sets the external connection DataSource type.

```javascript
setType(value: ConnectionDataSourceType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConnectionDataSourceType](./connectiondatasourcetype/) | The value to set. |

### getSourceFile() {#getSourceFile--}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

```javascript
getSourceFile() : string;
```


### setSourceFile(string) {#setSourceFile-string-}

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

```javascript
setSourceFile(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSSOId() {#getSSOId--}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

```javascript
getSSOId() : string;
```


### setSSOId(string) {#setSSOId-string-}

Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

```javascript
setSSOId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSavePassword() {#getSavePassword--}

True if the password is to be saved as part of the connection string; otherwise, False.

```javascript
getSavePassword() : boolean;
```


### setSavePassword(boolean) {#setSavePassword-boolean-}

True if the password is to be saved as part of the connection string; otherwise, False.

```javascript
setSavePassword(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSaveData() {#getSaveData--}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

```javascript
getSaveData() : boolean;
```


### setSaveData(boolean) {#setSaveData-boolean-}

True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

```javascript
setSaveData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshOnLoad() {#getRefreshOnLoad--}

True if this connection should be refreshed when opening the file; otherwise, false.

```javascript
getRefreshOnLoad() : boolean;
```


### setRefreshOnLoad(boolean) {#setRefreshOnLoad-boolean-}

True if this connection should be refreshed when opening the file; otherwise, false.

```javascript
setRefreshOnLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReconnectionMethodType() {#getReconnectionMethodType--}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.

```javascript
getReconnectionMethodType() : ReConnectionMethodType;
```


**Returns**

[ReConnectionMethodType](./reconnectionmethodtype/)

### setReconnectionMethodType(ReConnectionMethodType) {#setReconnectionMethodType-reconnectionmethodtype-}

Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.

```javascript
setReconnectionMethodType(value: ReConnectionMethodType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReConnectionMethodType](./reconnectionmethodtype/) | The value to set. |

### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

```javascript
getOnlyUseConnectionFile() : boolean;
```


### setOnlyUseConnectionFile(boolean) {#setOnlyUseConnectionFile-boolean-}

Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed.  If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

```javascript
setOnlyUseConnectionFile(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOdcFile() {#getOdcFile--}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

```javascript
getOdcFile() : string;
```


### setOdcFile(string) {#setOdcFile-string-}

Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

```javascript
setOdcFile(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isNew() {#isNew--}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

```javascript
isNew() : boolean;
```


### setIsNew(boolean) {#setIsNew-boolean-}

True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

```javascript
setIsNew(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getName() {#getName--}

Specifies the name of the connection. Each connection must have a unique name.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Specifies the name of the connection. Each connection must have a unique name.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getKeepAlive() {#getKeepAlive--}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

```javascript
getKeepAlive() : boolean;
```


### setKeepAlive(boolean) {#setKeepAlive-boolean-}

True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

```javascript
setKeepAlive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshInternal() {#getRefreshInternal--}

Specifies the number of minutes between automatic refreshes of the connection.

```javascript
getRefreshInternal() : number;
```


### setRefreshInternal(number) {#setRefreshInternal-number-}

Specifies the number of minutes between automatic refreshes of the connection.

```javascript
setRefreshInternal(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getConnectionId() {#getConnectionId--}

Specifies The unique identifier of this connection.

```javascript
getConnectionId() : number;
```


### getConnectionDescription() {#getConnectionDescription--}

Specifies the user description for this connection

```javascript
getConnectionDescription() : string;
```


### setConnectionDescription(string) {#setConnectionDescription-string-}

Specifies the user description for this connection

```javascript
setConnectionDescription(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isDeleted() {#isDeleted--}

Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false.

```javascript
isDeleted() : boolean;
```


### setIsDeleted(boolean) {#setIsDeleted-boolean-}

Indicates whether the associated workbook connection has been deleted.  true if the connection has been deleted; otherwise, false.

```javascript
setIsDeleted(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCredentialsMethodType() {#getCredentialsMethodType--}

Specifies the authentication method to be used when establishing (or re-establishing) the connection.

```javascript
getCredentialsMethodType() : CredentialsMethodType;
```


**Returns**

[CredentialsMethodType](./credentialsmethodtype/)

### setCredentialsMethodType(CredentialsMethodType) {#setCredentialsMethodType-credentialsmethodtype-}

Specifies the authentication method to be used when establishing (or re-establishing) the connection.

```javascript
setCredentialsMethodType(value: CredentialsMethodType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CredentialsMethodType](./credentialsmethodtype/) | The value to set. |

### getBackgroundRefresh() {#getBackgroundRefresh--}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

```javascript
getBackgroundRefresh() : boolean;
```


### setBackgroundRefresh(boolean) {#setBackgroundRefresh-boolean-}

Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

```javascript
setBackgroundRefresh(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getParameters() {#getParameters--}

Gets [ConnectionParameterCollection](./connectionparametercollection/) for an ODBC or web query.

```javascript
getParameters() : ConnectionParameterCollection;
```


**Returns**

[ConnectionParameterCollection](./connectionparametercollection/)

### getPowerQueryFormula() {#getPowerQueryFormula--}

Gets the definition of power query formula.

```javascript
getPowerQueryFormula() : PowerQueryFormula;
```


**Returns**

[PowerQueryFormula](./powerqueryformula/)


