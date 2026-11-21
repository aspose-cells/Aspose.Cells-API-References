---
title: "DataModelConnection"
second_title: "Aspose.Cells för Java API-referens"
description: "Anger en datamodellsanslutning"
type: docs
url: /sv/java/com.aspose.cells/datamodelconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class DataModelConnection extends ExternalConnection
```

Anger en datamodellsanslutning
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Anger om anslutningen kan uppdateras i bakgrunden (asynkront). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Hämtar typen av detta [ExternalConnection](../../com.aspose.cells/externalconnection) objekt. |
| [getCommand()](#getCommand--) | Strängen som innehåller databaskommandot att skicka till dataleverantörens API som kommer att interagera med den externa källan för att hämta data |
| [getCommandType()](#getCommandType--) | Returnerar [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) typ. |
| [getConnectionDescription()](#getConnectionDescription--) | Anger användarbeskrivningen för denna anslutning |
| [getConnectionFile()](#getConnectionFile--) | Hämtar anslutningsfilen. |
| [getConnectionId()](#getConnectionId--) | Anger den unika identifieraren för denna anslutning. |
| [getConnectionString()](#getConnectionString--) | Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla. |
| [getCredentials()](#getCredentials--) | Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). |
| [getId()](#getId--) | Hämtar id‑t för anslutningen. |
| [getKeepAlive()](#getKeepAlive--) | Sant när kalkylbladsprogrammet bör göra ansträngningar för att hålla anslutningen öppen. |
| [getName()](#getName--) | Anger namnet på anslutningen. |
| [getOdcFile()](#getOdcFile--) | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Anger om kalkylbladsprogrammet alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile‑attributet när anslutningen uppdateras. |
| [getParameters()](#getParameters--) | Hämtar [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) för en ODBC- eller webbfråga. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Hämtar definitionen av Power Query‑formeln. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Specificerar vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Specificerar vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. |
| [getRefreshInternal()](#getRefreshInternal--) | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | Sant om denna anslutning ska uppdateras när filen öppnas; annars falskt. |
| [getSSOId()](#getSSOId--) | Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan. |
| [getSaveData()](#getSaveData--) | Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars falskt. |
| [getSavePassword()](#getSavePassword--) | Sant om lösenordet ska sparas som en del av anslutningssträngen; annars falskt. |
| [getSecondCommand()](#getSecondCommand--) | Anger en andra kommandotextsträng som bevaras när pivottabellens serverbaserade sidfält används. |
| [getSourceFile()](#getSourceFile--) | Används när den externa datakällan är filbaserad. |
| [getSourceType()](#getSourceType--) | Hämtar den externa anslutningens DataSource‑typ. |
| [getType()](#getType--) | Hämtar den externa anslutningens DataSource‑typ. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | Anger om den associerade arbetsbokanslutningen har raderats. |
| [isNew()](#isNew--) | Sant om anslutningen inte har uppdaterats för första gången; annars falskt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Anger om anslutningen kan uppdateras i bakgrunden (asynkront). |
| [setCommand(String value)](#setCommand-java.lang.String-) | Strängen som innehåller databaskommandot att skicka till dataleverantörens API som kommer att interagera med den externa källan för att hämta data |
| [setCommandType(int value)](#setCommandType-int-) | Returnerar [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) typ. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Anger användarbeskrivningen för denna anslutning |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla. |
| [setCredentials(int value)](#setCredentials-int-) | Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Anger om den associerade arbetsbokanslutningen har raderats. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Sant när kalkylbladsprogrammet bör göra ansträngningar för att hålla anslutningen öppen. |
| [setName(String value)](#setName-java.lang.String-) | Anger namnet på anslutningen. |
| [setNew(boolean value)](#setNew-boolean-) | Sant om anslutningen inte har uppdaterats för första gången; annars falskt. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Anger om kalkylbladsprogrammet alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile‑attributet när anslutningen uppdateras. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Specificerar vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Specificerar vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Sant om denna anslutning ska uppdateras när filen öppnas; annars falskt. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars falskt. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Sant om lösenordet ska sparas som en del av anslutningssträngen; annars falskt. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Anger en andra kommandotextsträng som bevaras när pivottabellens serverbaserade sidfält används. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Används när den externa datakällan är filbaserad. |
| [setSourceType(int value)](#setSourceType-int-) | Ställer in den externa anslutningens DataSource-typ. |
| [setType(int value)](#setType-int-) | Ställer in den externa anslutningens DataSource-typ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Anger om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden.

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


Hämtar typen av detta [ExternalConnection](../../com.aspose.cells/externalconnection) objekt.

Se [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


Strängen som innehåller databaskommandot att skicka till dataleverantörens API som kommer att interagera med den externa källan för att hämta data

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Returnerar [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) typ.

Se [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Anger användarbeskrivningen för denna anslutning

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Hämtar anslutningsfilen.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Anger den unika identifieraren för denna anslutning.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.Id. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras).

Se [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.CredentialsMethodType. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras).

Se [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Hämtar id‑t för anslutningen.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


Sant när kalkylbladsapplikationen bör göra ansträngningar för att hålla anslutningen öppen. När falskt ska applikationen stänga anslutningen efter att ha hämtat informationen.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Anger anslutningens namn. Varje anslutning måste ha ett unikt namn.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Anger om kalkylbladsapplikationen alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om falskt ska kalkylbladsapplikationen följa proceduren som anges av reconnectionMethod-attributet.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Hämtar [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) för en ODBC- eller webbfråga.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Hämtar definitionen av Power Query‑formeln.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.

Se [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.ReconnectionMethodType. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.

Se [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Anger antalet minuter mellan automatiska uppdateringar av anslutningen.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


Sant om denna anslutning ska uppdateras när filen öppnas; annars falskt.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars falskt.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


Sant om lösenordet ska sparas som en del av anslutningssträngen; annars falskt.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


Anger en andra kommandotextsträng som sparas när PivotTable‑serverbaserade sidfält används. För ODBC‑anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE‑klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor kan konstrueras.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsprogrammet ansluta direkt till den här filen. Kan uttryckas i URI‑ eller systemspecifik filsökvägsnotation.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Hämtar den externa anslutningens DataSource‑typ.

Se [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Hämtar den externa anslutningens DataSource‑typ.

Se [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.SourceType. Denna egenskap kommer att tas bort 12 månader senare, från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Anger om den associerade arbetsboksanslutningen har raderats. true om anslutningen har raderats; annars false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True om anslutningen inte har uppdaterats för första gången; annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutförts.

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


Anger om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Strängen som innehåller databaskommandot att skicka till dataleverantörens API som kommer att interagera med den externa källan för att hämta data

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Returnerar [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype) typ.

Se [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Anger användarbeskrivningen för denna anslutning

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras).

Se [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.CredentialsMethodType. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras).

Se [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Anger om den associerade arbetsboksanslutningen har raderats. true om anslutningen har raderats; annars false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


Sant när kalkylbladsapplikationen bör göra ansträngningar för att hålla anslutningen öppen. När falskt ska applikationen stänga anslutningen efter att ha hämtat informationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Anger anslutningens namn. Varje anslutning måste ha ett unikt namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


True om anslutningen inte har uppdaterats för första gången; annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutförts.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Anger om kalkylbladsapplikationen alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om falskt ska kalkylbladsapplikationen följa proceduren som anges av reconnectionMethod-attributet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.

Se [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.ReconnectionMethodType. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.

Se [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Anger antalet minuter mellan automatiska uppdateringar av anslutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


Sant om denna anslutning ska uppdateras när filen öppnas; annars falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


Sant om lösenordet ska sparas som en del av anslutningssträngen; annars falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


Anger en andra kommandotextsträng som sparas när PivotTable‑serverbaserade sidfält används. För ODBC‑anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE‑klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor kan konstrueras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsprogrammet ansluta direkt till den här filen. Kan uttryckas i URI‑ eller systemspecifik filsökvägsnotation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Ställer in den externa anslutningens DataSource-typ.

Se [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Ställer in den externa anslutningens DataSource-typ.

Se [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen ExternalConnection.SourceType. Denna egenskap kommer att tas bort 12 månader senare, från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

