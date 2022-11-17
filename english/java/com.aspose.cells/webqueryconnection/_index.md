---
title: WebQueryConnection
second_title: Aspose.Cells for Java API Reference
description: Specifies the properties for a web query source.
type: docs
weight: 652
url: /java/com.aspose.cells/webqueryconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class WebQueryConnection extends ExternalConnection
```

Specifies the properties for a web query source. A web query will retrieve data from HTML tables, and can also supply HTTP "Get" parameters to be processed by the web server in generating the HTML by including the parameters and parameter elements.
## Constructors

| Constructor | Description |
| --- | --- |
| [WebQueryConnection()](#WebQueryConnection--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Indicates whether the connection can be refreshed in the background (asynchronously). |
| [getClass()](#getClass--) |  |
| [getConnectionDescription()](#getConnectionDescription--) | Specifies the user description for this connection |
| [getConnectionId()](#getConnectionId--) | Specifies The unique identifier of this connection. |
| [getCredentials()](#getCredentials--) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Specifies the authentication method to be used when establishing (or re-establishing) the connection. |
| [getEditPage()](#getEditPage--) | The URL of the user-facing web page showing the web query data. |
| [getEditWebPage()](#getEditWebPage--) | The URL of the user-facing web page showing the web query data. |
| [getHtmlFormat()](#getHtmlFormat--) | How to handle formatting from the HTML source when bringing web query data into the worksheet. |
| [getId()](#getId--) | Gets the id of the connection. |
| [getKeepAlive()](#getKeepAlive--) | True when the spreadsheet application should make efforts to keep the connection open. |
| [getName()](#getName--) | Specifies the name of the connection. |
| [getOdcFile()](#getOdcFile--) | Specifies the full path to external connection file from which this connection was created. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. |
| [getParameters()](#getParameters--) | Gets [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) for an ODBC or web query. |
| [getPost()](#getPost--) | Returns or sets the string used with the post method of inputting data into a web server to return data from a web query. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Gets the definition of power query formula. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Specifies what the spreadsheet application should do when a connection fails. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Specifies what the spreadsheet application should do when a connection fails. |
| [getRefreshInternal()](#getRefreshInternal--) | Specifies the number of minutes between automatic refreshes of the connection. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | True if this connection should be refreshed when opening the file; otherwise, false. |
| [getSSOId()](#getSSOId--) | Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source. |
| [getSaveData()](#getSaveData--) | True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false. |
| [getSavePassword()](#getSavePassword--) | True if the password is to be saved as part of the connection string; otherwise, False. |
| [getSourceFile()](#getSourceFile--) | Used when the external data source is file-based. |
| [getType()](#getType--) | Gets or Sets the external connection DataSource type. |
| [getUrl()](#getUrl--) | URL to use to refresh external data. |
| [hashCode()](#hashCode--) |  |
| [isConsecutive()](#isConsecutive--) | Flag indicating whether consecutive delimiters should be treated as just one delimiter. |
| [isDeleted()](#isDeleted--) | Indicates whether the associated workbook connection has been deleted. |
| [isHtmlTables()](#isHtmlTables--) | Flag indicating whether web queries should only work on HTML tables. |
| [isNew()](#isNew--) | True if the connection has not been refreshed for the first time; otherwise, false. |
| [isParsePre()](#isParsePre--) | Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table. |
| [isSameSettings()](#isSameSettings--) | Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row. |
| [isTextDates()](#isTextDates--) | Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates. |
| [isXl2000()](#isXl2000--) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. |
| [isXl97()](#isXl97--) | This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. |
| [isXml()](#isXml--) | true if the web query source is XML (versus HTML), otherwise false. |
| [isXmlSourceData()](#isXmlSourceData--) | Flag indicating that XML source data should be imported instead of the HTML table itself. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) |  |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) |  |
| [setConsecutive(boolean value)](#setConsecutive-boolean-) |  |
| [setCredentials(int value)](#setCredentials-int-) |  |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) |  |
| [setDeleted(boolean value)](#setDeleted-boolean-) |  |
| [setEditPage(String value)](#setEditPage-java.lang.String-) |  |
| [setEditWebPage(String value)](#setEditWebPage-java.lang.String-) |  |
| [setHtmlFormat(int value)](#setHtmlFormat-int-) |  |
| [setHtmlTables(boolean value)](#setHtmlTables-boolean-) |  |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) |  |
| [setName(String value)](#setName-java.lang.String-) |  |
| [setNew(boolean value)](#setNew-boolean-) |  |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) |  |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) |  |
| [setParsePre(boolean value)](#setParsePre-boolean-) |  |
| [setPost(String value)](#setPost-java.lang.String-) |  |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) |  |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) |  |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) |  |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) |  |
| [setSSOId(String value)](#setSSOId-java.lang.String-) |  |
| [setSameSettings(boolean value)](#setSameSettings-boolean-) |  |
| [setSaveData(boolean value)](#setSaveData-boolean-) |  |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) |  |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) |  |
| [setTextDates(boolean value)](#setTextDates-boolean-) |  |
| [setType(int value)](#setType-int-) |  |
| [setUrl(String value)](#setUrl-java.lang.String-) |  |
| [setXl2000(boolean value)](#setXl2000-boolean-) |  |
| [setXl97(boolean value)](#setXl97-boolean-) |  |
| [setXml(boolean value)](#setXml-boolean-) |  |
| [setXmlSourceData(boolean value)](#setXmlSourceData-boolean-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WebQueryConnection() {#WebQueryConnection--}
```
public WebQueryConnection()
```


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
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Indicates whether the connection can be refreshed in the background (asynchronously). true if preferred usage of the connection is to refresh asynchronously in the background; false if preferred usage of the connection is to refresh synchronously in the foreground.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Specifies the user description for this connection

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Specifies The unique identifier of this connection.

**Returns:**
int
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Specifies the authentication method to be used when establishing (or re-establishing) the connection. NOTE: This property is now obsolete. Instead, please use ExternalConnection.CredentialsMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Specifies the authentication method to be used when establishing (or re-establishing) the connection.

**Returns:**
int
### getEditPage() {#getEditPage--}
```
public String getEditPage()
```


The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes. NOTE: This property is now obsolete. Instead, please use WebQueryConnection.EditWebPage property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getEditWebPage() {#getEditWebPage--}
```
public String getEditWebPage()
```


The URL of the user-facing web page showing the web query data. This URL is persisted in the case that sourceData="true" and url has been redirected to reference an XML file. Then the user-facing page can be shown in the UI, and the XML data can be retrieved behind the scenes.

**Returns:**
java.lang.String
### getHtmlFormat() {#getHtmlFormat--}
```
public int getHtmlFormat()
```


How to handle formatting from the HTML source when bringing web query data into the worksheet. Relevant when sourceData is True.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Gets the id of the connection.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


True when the spreadsheet application should make efforts to keep the connection open. When false, the application should close the connection after retrieving the information.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Specifies the name of the connection. Each connection must have a unique name.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Indicates whether the spreadsheet application should always and only use the connection information in the external connection file indicated by the odcFile attribute when the connection is refreshed. If false, then the spreadsheet application should follow the procedure indicated by the reconnectionMethod attribute

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Gets [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) for an ODBC or web query.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPost() {#getPost--}
```
public String getPost()
```


Returns or sets the string used with the post method of inputting data into a web server to return data from a web query.

**Returns:**
java.lang.String
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Gets the definition of power query formula.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required. NOTE: This property is now obsolete. Instead, please use ExternalConnection.ReconnectionMethodType property. This property will be removed 12 months later since October 2017. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Specifies what the spreadsheet application should do when a connection fails. The default value is ReConnectionMethodType.Required.

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Specifies the number of minutes between automatic refreshes of the connection.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


True if this connection should be refreshed when opening the file; otherwise, false.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


True if the password is to be saved as part of the connection string; otherwise, False.

**Returns:**
boolean
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Gets or Sets the external connection DataSource type.

**Returns:**
int
### getUrl() {#getUrl--}
```
public String getUrl()
```


URL to use to refresh external data.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isConsecutive() {#isConsecutive--}
```
public boolean isConsecutive()
```


Flag indicating whether consecutive delimiters should be treated as just one delimiter.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.

**Returns:**
boolean
### isHtmlTables() {#isHtmlTables--}
```
public boolean isHtmlTables()
```


Flag indicating whether web queries should only work on HTML tables.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.

**Returns:**
boolean
### isParsePre() {#isParsePre--}
```
public boolean isParsePre()
```


Flag indicating whether data contained within HTML PRE tags in the web page is parsed into columns when you import the page into a query table.

**Returns:**
boolean
### isSameSettings() {#isSameSettings--}
```
public boolean isSameSettings()
```


Flag indicating whether to parse all tables inside a PRE block with the same width settings as the first row.

**Returns:**
boolean
### isTextDates() {#isTextDates--}
```
public boolean isTextDates()
```


Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates.

**Returns:**
boolean
### isXl2000() {#isXl2000--}
```
public boolean isXl2000()
```


This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was refreshed in a spreadsheet application newer than or equal to Microsoft Excel 2000. This is an optional attribute that can be ignored.

**Returns:**
boolean
### isXl97() {#isXl97--}
```
public boolean isXl97()
```


This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored.

**Returns:**
boolean
### isXml() {#isXml--}
```
public boolean isXml()
```


true if the web query source is XML (versus HTML), otherwise false.

**Returns:**
boolean
### isXmlSourceData() {#isXmlSourceData--}
```
public boolean isXmlSourceData()
```


Flag indicating that XML source data should be imported instead of the HTML table itself.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundRefresh(boolean value) {#setBackgroundRefresh-boolean-}
```
public void setBackgroundRefresh(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setConsecutive(boolean value) {#setConsecutive-boolean-}
```
public void setConsecutive(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEditPage(String value) {#setEditPage-java.lang.String-}
```
public void setEditPage(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setEditWebPage(String value) {#setEditWebPage-java.lang.String-}
```
public void setEditWebPage(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setHtmlFormat(int value) {#setHtmlFormat-int-}
```
public void setHtmlFormat(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHtmlTables(boolean value) {#setHtmlTables-boolean-}
```
public void setHtmlTables(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setParsePre(boolean value) {#setParsePre-boolean-}
```
public void setParsePre(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPost(String value) {#setPost-java.lang.String-}
```
public void setPost(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setSameSettings(boolean value) {#setSameSettings-boolean-}
```
public void setSameSettings(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextDates(boolean value) {#setTextDates-boolean-}
```
public void setTextDates(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUrl(String value) {#setUrl-java.lang.String-}
```
public void setUrl(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setXl2000(boolean value) {#setXl2000-boolean-}
```
public void setXl2000(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setXl97(boolean value) {#setXl97-boolean-}
```
public void setXl97(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setXml(boolean value) {#setXml-boolean-}
```
public void setXml(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setXmlSourceData(boolean value) {#setXmlSourceData-boolean-}
```
public void setXmlSourceData(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

