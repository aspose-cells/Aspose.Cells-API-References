---
title: "ExternalConnection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает внешнее подключение данных"
type: docs
url: /ru/java/com.aspose.cells/externalconnection/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExternalConnection
```

Указывает внешнее подключение данных
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Получает тип этого объекта [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getCommand()](#getCommand--) | Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных. |
| [getCommandType()](#getCommandType--) | Указывает тип команды OLE DB. 1. |
| [getConnectionDescription()](#getConnectionDescription--) | Указывает пользовательское описание для этого соединения. |
| [getConnectionFile()](#getConnectionFile--) | Получает файл соединения. |
| [getConnectionId()](#getConnectionId--) | Указывает уникальный идентификатор этого соединения. |
| [getConnectionString()](#getConnectionString--) | Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC. |
| [getCredentials()](#getCredentials--) | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. |
| [getId()](#getId--) | Получает идентификатор соединения. |
| [getKeepAlive()](#getKeepAlive--) | True, когда приложение электронных таблиц должно прилагать усилия для поддержания соединения открытым. |
| [getName()](#getName--) | Указывает имя соединения. |
| [getOdcFile()](#getOdcFile--) | Указывает полный путь к внешнему файлу соединения, из которого было создано это соединение. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Указывает, должно ли приложение электронных таблиц всегда и исключительно использовать информацию о соединении во внешнем файле соединения, указанном атрибутом odcFile, при обновлении соединения. |
| [getParameters()](#getParameters--) | Получает [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) для ODBC или веб‑запроса. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Получает определение формулы Power Query. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Указывает, что должно делать приложение электронной таблицы при сбое соединения. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Указывает, что должно делать приложение электронной таблицы при сбое соединения. |
| [getRefreshInternal()](#getRefreshInternal--) | Указывает количество минут между автоматическими обновлениями соединения. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | True, если это соединение должно обновляться при открытии файла; в противном случае false. |
| [getSSOId()](#getSSOId--) | Идентификатор для Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных. |
| [getSaveData()](#getSaveData--) | True, если внешние данные, полученные через соединение для заполнения таблицы, должны сохраняться вместе с книгой; в противном случае false. |
| [getSavePassword()](#getSavePassword--) | True, если пароль должен сохраняться как часть строки соединения; в противном случае False. |
| [getSecondCommand()](#getSecondCommand--) | Указывает вторую строку текста команды, которая сохраняется, когда используются полевые параметры PivotTable на основе сервера. |
| [getSourceFile()](#getSourceFile--) | Используется, когда внешний источник данных основан на файле. |
| [getSourceType()](#getSourceType--) | Получает тип внешнего соединения DataSource. |
| [getType()](#getType--) | Получает тип внешнего соединения DataSource. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | Указывает, было ли удалено связанное соединение книги. |
| [isNew()](#isNew--) | True, если соединение не было обновлено впервые; в противном случае — false. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). |
| [setCommand(String value)](#setCommand-java.lang.String-) | Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных. |
| [setCommandType(int value)](#setCommandType-int-) | Указывает тип команды OLE DB. 1. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Указывает пользовательское описание для этого соединения. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC. |
| [setCredentials(int value)](#setCredentials-int-) | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Указывает, было ли удалено связанное соединение книги. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | True, когда приложение электронных таблиц должно прилагать усилия для поддержания соединения открытым. |
| [setName(String value)](#setName-java.lang.String-) | Указывает имя соединения. |
| [setNew(boolean value)](#setNew-boolean-) | True, если соединение не было обновлено впервые; в противном случае — false. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Указывает полный путь к внешнему файлу соединения, из которого было создано это соединение. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Указывает, должно ли приложение электронных таблиц всегда и исключительно использовать информацию о соединении во внешнем файле соединения, указанном атрибутом odcFile, при обновлении соединения. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Указывает, что должно делать приложение электронной таблицы при сбое соединения. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Указывает, что должно делать приложение электронной таблицы при сбое соединения. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Указывает количество минут между автоматическими обновлениями соединения. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | True, если это соединение должно обновляться при открытии файла; в противном случае false. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Идентификатор для Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | True, если внешние данные, полученные через соединение для заполнения таблицы, должны сохраняться вместе с книгой; в противном случае false. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | True, если пароль должен сохраняться как часть строки соединения; в противном случае False. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Указывает вторую строку текста команды, которая сохраняется, когда используются полевые параметры PivotTable на основе сервера. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Используется, когда внешний источник данных основан на файле. |
| [setSourceType(int value)](#setSourceType-int-) | Устанавливает тип внешнего соединения DataSource. |
| [setType(int value)](#setType-int-) | Устанавливает тип внешнего соединения DataSource. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно в переднем плане.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClassType() {#getClassType--}
```
public abstract int getClassType()
```


Получает тип этого объекта [ExternalConnection](../../com.aspose.cells/externalconnection).

См. [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика. 5. Запрос направлен к веб‑ориентированному поставщику List Data Provider.

См. [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Указывает пользовательское описание для этого соединения.

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Получает файл соединения.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Указывает уникальный идентификатор этого соединения.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство ExternalConnection.Id. Это свойство будет удалено через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения.

См. [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство ExternalConnection.CredentialsMethodType. Это свойство будет удалено через 12 месяцев, начиная с октября 2017 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения.

См. [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Получает идентификатор соединения.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


True, когда приложение электронных таблиц должно стараться держать соединение открытым. Когда false, приложение должно закрыть соединение после получения информации.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Указывает имя соединения. Каждое соединение должно иметь уникальное имя.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Указывает полный путь к внешнему файлу соединения, из которого было создано данное соединение. Если соединение не удаётся во время попытки обновления данных, и reconnectionMethod=1, приложение электронных таблиц попробует снова, используя информацию из внешнего файла соединения вместо встроенного в книгу объекта соединения.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Указывает, должно ли приложение электронных таблиц всегда и исключительно использовать информацию о соединении из внешнего файла соединения, указанного атрибутом odcFile, при обновлении соединения. Если false, приложение должно следовать процедуре, указанной атрибутом reconnectionMethod.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Получает [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) для ODBC или веб‑запроса.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Получает определение формулы Power Query.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required.

См. [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство ExternalConnection.ReconnectionMethodType. Это свойство будет удалено через 12 месяцев, начиная с октября 2017 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required.

См. [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Указывает количество минут между автоматическими обновлениями соединения.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


True, если это соединение должно обновляться при открытии файла; в противном случае false.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Идентификатор для Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


True, если внешние данные, полученные через соединение для заполнения таблицы, должны сохраняться вместе с книгой; в противном случае false.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


True, если пароль должен сохраняться как часть строки соединения; в противном случае False.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


Указывает вторую строку текста команды, которая сохраняется при использовании серверных полей страниц PivotTable. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command (в первом отсутствует условие WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Используется, когда внешний источник данных основан на файле. Когда соединение с таким источником данных не удаётся, приложение электронных таблиц пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно‑специфической нотации пути к файлу.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Получает тип внешнего соединения DataSource.

Смотрите [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Получает тип внешнего соединения DataSource.

Смотрите [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ExternalConnection.SourceType. Это свойство будет удалено через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Указывает, удалено ли связанное соединение книги. true, если соединение было удалено; иначе false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True, если соединение ещё не было обновлено впервые; иначе false. Это состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса.

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


Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно в переднем плане.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика. 5. Запрос направлен к веб‑ориентированному поставщику List Data Provider.

См. [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Указывает пользовательское описание для этого соединения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения.

См. [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство ExternalConnection.CredentialsMethodType. Это свойство будет удалено через 12 месяцев, начиная с октября 2017 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения.

См. [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Указывает, удалено ли связанное соединение книги. true, если соединение было удалено; иначе false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


True, когда приложение электронных таблиц должно стараться держать соединение открытым. Когда false, приложение должно закрыть соединение после получения информации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Указывает имя соединения. Каждое соединение должно иметь уникальное имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


True, если соединение ещё не было обновлено впервые; иначе false. Это состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Указывает полный путь к внешнему файлу соединения, из которого было создано данное соединение. Если соединение не удаётся во время попытки обновления данных, и reconnectionMethod=1, приложение электронных таблиц попробует снова, используя информацию из внешнего файла соединения вместо встроенного в книгу объекта соединения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Указывает, должно ли приложение электронных таблиц всегда и исключительно использовать информацию о соединении из внешнего файла соединения, указанного атрибутом odcFile, при обновлении соединения. Если false, приложение должно следовать процедуре, указанной атрибутом reconnectionMethod.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required.

См. [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство ExternalConnection.ReconnectionMethodType. Это свойство будет удалено через 12 месяцев, начиная с октября 2017 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required.

См. [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Указывает количество минут между автоматическими обновлениями соединения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


True, если это соединение должно обновляться при открытии файла; в противном случае false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Идентификатор для Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


True, если внешние данные, полученные через соединение для заполнения таблицы, должны сохраняться вместе с книгой; в противном случае false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


True, если пароль должен сохраняться как часть строки соединения; в противном случае False.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


Указывает вторую строку текста команды, которая сохраняется при использовании серверных полей страниц PivotTable. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command (в первом отсутствует условие WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Используется, когда внешний источник данных основан на файле. Когда соединение с таким источником данных не удаётся, приложение электронных таблиц пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно‑специфической нотации пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Устанавливает тип внешнего соединения DataSource.

Смотрите [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип внешнего соединения DataSource.

Смотрите [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ExternalConnection.SourceType. Это свойство будет удалено через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

