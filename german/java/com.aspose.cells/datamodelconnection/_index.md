---
title: "DataModelConnection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt eine Datenmodellverbindung an"
type: docs
url: /de/java/com.aspose.cells/datamodelconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class DataModelConnection extends ExternalConnection
```

Gibt eine Datenmodellverbindung an
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Ermittelt den Typ dieses [ExternalConnection](../../com.aspose.cells/externalconnection)-Objekts. |
| [getCommand()](#getCommand--) | Die Zeichenfolge, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen |
| [getCommandType()](#getCommandType--) | Gibt den Typ [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) zurück. |
| [getConnectionDescription()](#getConnectionDescription--) | Gibt die Benutzerbeschreibung für diese Verbindung an |
| [getConnectionFile()](#getConnectionFile--) | Ermittelt die Verbindungsdatei. |
| [getConnectionId()](#getConnectionId--) | Gibt die eindeutige Kennung dieser Verbindung an. |
| [getConnectionString()](#getConnectionString--) | Die Verbindungsinformationszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. |
| [getCredentials()](#getCredentials--) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [getId()](#getId--) | Ermittelt die ID der Verbindung. |
| [getKeepAlive()](#getKeepAlive--) | True, wenn die Tabellenkalkulationsanwendung Anstrengungen unternehmen soll, die Verbindung offen zu halten. |
| [getName()](#getName--) | Gibt den Namen der Verbindung an. |
| [getOdcFile()](#getOdcFile--) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets und ausschließlich die Verbindungsinformationen in der durch das Attribut odcFile angegebenen externen Verbindungsdatei verwenden soll. |
| [getParameters()](#getParameters--) | Ermittelt die [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) für eine ODBC- oder Webabfrage. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Ermittelt die Definition der Power‑Query‑Formel. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. |
| [getRefreshInternal()](#getRefreshInternal--) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false. |
| [getSSOId()](#getSSOId--) | Kennung für Single Sign‑On (SSO), das für die Authentifizierung zwischen einem Zwischenspeicher‑SpreadsheetML‑Server und der externen Datenquelle verwendet wird. |
| [getSaveData()](#getSaveData--) | True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false. |
| [getSavePassword()](#getSavePassword--) | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False. |
| [getSecondCommand()](#getSecondCommand--) | Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. |
| [getSourceFile()](#getSourceFile--) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. |
| [getSourceType()](#getSourceType--) | Ermittelt den DataSource‑Typ der externen Verbindung. |
| [getType()](#getType--) | Ermittelt den DataSource‑Typ der externen Verbindung. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. |
| [isNew()](#isNew--) | True wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Die Zeichenfolge, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen |
| [setCommandType(int value)](#setCommandType-int-) | Gibt den Typ [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) zurück. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Gibt die Benutzerbeschreibung für diese Verbindung an |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Die Verbindungsinformationszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. |
| [setCredentials(int value)](#setCredentials-int-) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | True, wenn die Tabellenkalkulationsanwendung Anstrengungen unternehmen soll, die Verbindung offen zu halten. |
| [setName(String value)](#setName-java.lang.String-) | Gibt den Namen der Verbindung an. |
| [setNew(boolean value)](#setNew-boolean-) | True wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets und ausschließlich die Verbindungsinformationen in der durch das Attribut odcFile angegebenen externen Verbindungsdatei verwenden soll. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Kennung für Single Sign‑On (SSO), das für die Authentifizierung zwischen einem Zwischenspeicher‑SpreadsheetML‑Server und der externen Datenquelle verwendet wird. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. |
| [setSourceType(int value)](#setSourceType-int-) | Legt den Typ der externen Verbindungs‑DataSource fest. |
| [setType(int value)](#setType-int-) | Legt den Typ der externen Verbindungs‑DataSource fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Verwendung darin besteht, synchron im Vordergrund zu aktualisieren.

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
public int getClassType()
```


Ermittelt den Typ dieses [ExternalConnection](../../com.aspose.cells/externalconnection)-Objekts.

Siehe [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


Die Zeichenfolge, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Gibt den Typ [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) zurück.

Siehe [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Gibt die Benutzerbeschreibung für diese Verbindung an

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Ermittelt die Verbindungsdatei.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Gibt die eindeutige Kennung dieser Verbindung an.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.Id. Diese Eigenschaft wird 12 Monate nach Oktober 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


Die Verbindungsinformationszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.

Siehe [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.CredentialsMethodType. Diese Eigenschaft wird 12 Monate nach Oktober 2017 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.

Siehe [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Ermittelt die ID der Verbindung.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


True, wenn die Tabellenkalkulationsanwendung bemüht sein sollte, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1 ist, versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei anstelle des im Arbeitsbuch eingebetteten Verbindungsobjekts zu verwenden.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets ausschließlich die Verbindungsinformationen in der durch das Attribut odcFile angegebenen externen Verbindungsdatei verwenden soll. Wenn false, sollte die Anwendung dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Ermittelt die [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) für eine ODBC- oder Webabfrage.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Ermittelt die Definition der Power‑Query‑Formel.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required.

Siehe [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.ReconnectionMethodType. Diese Eigenschaft wird 12 Monate nach Oktober 2017 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required.

Siehe [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Kennung für Single Sign‑On (SSO), das für die Authentifizierung zwischen einem Zwischenspeicher‑SpreadsheetML‑Server und der externen Datenquelle verwendet wird.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn PivotTable-Server-basierte Seitenfelder verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfassendere Abfrage als command (bei der erstgenannten ist keine WHERE‑Klausel vorhanden). Basierend auf diesen beiden Befehlen (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann als URI oder in systemabhängiger Dateipfadnotation angegeben werden.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Ermittelt den DataSource‑Typ der externen Verbindung.

Siehe [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Ermittelt den DataSource‑Typ der externen Verbindung.

Siehe [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.SourceType. Diese Eigenschaft wird 12 Monate später, seit Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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


Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist.

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


Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Verwendung darin besteht, synchron im Vordergrund zu aktualisieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Die Zeichenfolge, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Gibt den Typ [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) zurück.

Siehe [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Gibt die Benutzerbeschreibung für diese Verbindung an

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


Die Verbindungsinformationszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.

Siehe [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.CredentialsMethodType. Diese Eigenschaft wird 12 Monate nach Oktober 2017 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.

Siehe [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


True, wenn die Tabellenkalkulationsanwendung bemüht sein sollte, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1 ist, versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei anstelle des im Arbeitsbuch eingebetteten Verbindungsobjekts zu verwenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets ausschließlich die Verbindungsinformationen in der durch das Attribut odcFile angegebenen externen Verbindungsdatei verwenden soll. Wenn false, sollte die Anwendung dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required.

Siehe [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.ReconnectionMethodType. Diese Eigenschaft wird 12 Monate nach Oktober 2017 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required.

Siehe [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Kennung für Single Sign‑On (SSO), das für die Authentifizierung zwischen einem Zwischenspeicher‑SpreadsheetML‑Server und der externen Datenquelle verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn PivotTable-Server-basierte Seitenfelder verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfassendere Abfrage als command (bei der erstgenannten ist keine WHERE‑Klausel vorhanden). Basierend auf diesen beiden Befehlen (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann als URI oder in systemabhängiger Dateipfadnotation angegeben werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Legt den Typ der externen Verbindungs‑DataSource fest.

Siehe [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Legt den Typ der externen Verbindungs‑DataSource fest.

Siehe [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.SourceType. Diese Eigenschaft wird 12 Monate später, seit Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

