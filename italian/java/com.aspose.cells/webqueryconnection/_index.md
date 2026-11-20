---
title: "WebQueryConnection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica le proprietà per una sorgente di query web."
type: docs
url: /it/java/com.aspose.cells/webqueryconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class WebQueryConnection extends ExternalConnection
```

Specifica le proprietà per una sorgente di query web. Una query web recupererà i dati dalle tabelle HTML e può anche fornire parametri HTTP "Get" da elaborare dal server web nella generazione dell'HTML includendo i parametri e gli elementi dei parametri.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Indica se la connessione può essere aggiornata in background (asincronicamente). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Restituisce il tipo di questo oggetto [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getCommand()](#getCommand--) | La stringa contenente il comando del database da passare all'API del provider di dati che interagirà con la fonte esterna per recuperare i dati. |
| [getCommandType()](#getCommandType--) | Specifica il tipo di comando OLE DB. 1. |
| [getConnectionDescription()](#getConnectionDescription--) | Specifica la descrizione dell'utente per questa connessione. |
| [getConnectionFile()](#getConnectionFile--) | Restituisce il file di connessione. |
| [getConnectionId()](#getConnectionId--) | Specifica l'identificatore univoco di questa connessione. |
| [getConnectionString()](#getConnectionString--) | La stringa di informazioni sulla connessione è utilizzata per stabilire un contatto con una fonte dati OLE DB o ODBC. |
| [getCredentials()](#getCredentials--) | Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione. |
| [getEditPage()](#getEditPage--) | L'URL della pagina web destinata all'utente che mostra i dati della query web. |
| [getEditWebPage()](#getEditWebPage--) | L'URL della pagina web destinata all'utente che mostra i dati della query web. |
| [getHtmlFormat()](#getHtmlFormat--) | Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. |
| [getId()](#getId--) | Restituisce l'ID della connessione. |
| [getKeepAlive()](#getKeepAlive--) | Vero quando l'applicazione di foglio di calcolo dovrebbe fare sforzi per mantenere la connessione aperta. |
| [getName()](#getName--) | Specifica il nome della connessione. |
| [getOdcFile()](#getOdcFile--) | Specifica il percorso completo al file di connessione esterno da cui è stata creata questa connessione. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Indica se l'applicazione di foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. |
| [getParameters()](#getParameters--) | Restituisce [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) per una query ODBC o web. |
| [getPost()](#getPost--) | Restituisce o imposta la stringa utilizzata con il metodo POST per inviare dati a un server web al fine di restituire i dati da una query web. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Restituisce la definizione della formula Power Query. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. |
| [getRefreshInternal()](#getRefreshInternal--) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | Vero se questa connessione deve essere aggiornata all'apertura del file; altrimenti, falso. |
| [getSSOId()](#getSSOId--) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermedio spreadsheetML e la fonte dati esterna. |
| [getSaveData()](#getSaveData--) | Vero se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, falso. |
| [getSavePassword()](#getSavePassword--) | Vero se la password deve essere salvata come parte della stringa di connessione; altrimenti, Falso. |
| [getSecondCommand()](#getSecondCommand--) | Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server PivotTable sono in uso. |
| [getSourceFile()](#getSourceFile--) | Utilizzato quando la fonte dati esterna è basata su file. |
| [getSourceType()](#getSourceType--) | Ottiene il tipo di DataSource della connessione esterna. |
| [getType()](#getType--) | Ottiene il tipo di DataSource della connessione esterna. |
| [getUrl()](#getUrl--) | URL da utilizzare per aggiornare i dati esterni. |
| [hashCode()](#hashCode--) |  |
| [isConsecutive()](#isConsecutive--) | Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore. |
| [isDeleted()](#isDeleted--) | Indica se la connessione della cartella di lavoro associata è stata eliminata. |
| [isHtmlTables()](#isHtmlTables--) | Flag che indica se le query web devono funzionare solo su tabelle HTML. |
| [isNew()](#isNew--) | True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. |
| [isParsePre()](#isParsePre--) | Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query. |
| [isSameSettings()](#isSameSettings--) | Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga. |
| [isTextDates()](#isTextDates--) | Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date. |
| [isXl2000()](#isXl2000--) | Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. |
| [isXl97()](#isXl97--) | Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata creata in Microsoft Excel 97. |
| [isXml()](#isXml--) | true se la sorgente della query web è XML (invece di HTML), altrimenti false. |
| [isXmlSourceData()](#isXmlSourceData--) | Flag che indica che i dati sorgente XML dovrebbero essere importati invece della tabella HTML stessa. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Indica se la connessione può essere aggiornata in background (asincronicamente). |
| [setCommand(String value)](#setCommand-java.lang.String-) | La stringa contenente il comando del database da passare all'API del provider di dati che interagirà con la fonte esterna per recuperare i dati. |
| [setCommandType(int value)](#setCommandType-int-) | Specifica il tipo di comando OLE DB. 1. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Specifica la descrizione dell'utente per questa connessione. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | La stringa di informazioni sulla connessione è utilizzata per stabilire un contatto con una fonte dati OLE DB o ODBC. |
| [setConsecutive(boolean value)](#setConsecutive-boolean-) | Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore. |
| [setCredentials(int value)](#setCredentials-int-) | Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indica se la connessione della cartella di lavoro associata è stata eliminata. |
| [setEditPage(String value)](#setEditPage-java.lang.String-) | L'URL della pagina web destinata all'utente che mostra i dati della query web. |
| [setEditWebPage(String value)](#setEditWebPage-java.lang.String-) | L'URL della pagina web destinata all'utente che mostra i dati della query web. |
| [setHtmlFormat(int value)](#setHtmlFormat-int-) | Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. |
| [setHtmlTables(boolean value)](#setHtmlTables-boolean-) | Flag che indica se le query web devono funzionare solo su tabelle HTML. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Vero quando l'applicazione di foglio di calcolo dovrebbe fare sforzi per mantenere la connessione aperta. |
| [setName(String value)](#setName-java.lang.String-) | Specifica il nome della connessione. |
| [setNew(boolean value)](#setNew-boolean-) | True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Specifica il percorso completo al file di connessione esterno da cui è stata creata questa connessione. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Indica se l'applicazione di foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. |
| [setParsePre(boolean value)](#setParsePre-boolean-) | Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query. |
| [setPost(String value)](#setPost-java.lang.String-) | Restituisce o imposta la stringa utilizzata con il metodo POST per inviare dati a un server web al fine di restituire i dati da una query web. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Vero se questa connessione deve essere aggiornata all'apertura del file; altrimenti, falso. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermedio spreadsheetML e la fonte dati esterna. |
| [setSameSettings(boolean value)](#setSameSettings-boolean-) | Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Vero se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, falso. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Vero se la password deve essere salvata come parte della stringa di connessione; altrimenti, Falso. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server PivotTable sono in uso. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Utilizzato quando la fonte dati esterna è basata su file. |
| [setSourceType(int value)](#setSourceType-int-) | Imposta il tipo di DataSource della connessione esterna. |
| [setTextDates(boolean value)](#setTextDates-boolean-) | Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date. |
| [setType(int value)](#setType-int-) | Imposta il tipo di DataSource della connessione esterna. |
| [setUrl(String value)](#setUrl-java.lang.String-) | URL da utilizzare per aggiornare i dati esterni. |
| [setXl2000(boolean value)](#setXl2000-boolean-) | Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. |
| [setXl97(boolean value)](#setXl97-boolean-) | Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata creata in Microsoft Excel 97. |
| [setXml(boolean value)](#setXml-boolean-) | true se la sorgente della query web è XML (invece di HTML), altrimenti false. |
| [setXmlSourceData(boolean value)](#setXmlSourceData-boolean-) | Flag che indica che i dati sorgente XML dovrebbero essere importati invece della tabella HTML stessa. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronamente in background; false se l'uso preferito della connessione è aggiornare sincronicamente in primo piano.

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


Restituisce il tipo di questo oggetto [ExternalConnection](../../com.aspose.cells/externalconnection).

Vedi [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


La stringa contenente il comando del database da passare all'API del provider di dati che interagirà con la fonte esterna per recuperare i dati.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Specifica il tipo di comando OLE DB. 1. La query specifica un nome di cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome di tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è rivolta a un provider di dati elenco basato sul web.

Vedi [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Specifica la descrizione dell'utente per questa connessione.

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Restituisce il file di connessione.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Specifica l'identificatore univoco di questa connessione.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.Id. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


La stringa di informazioni sulla connessione è utilizzata per stabilire un contatto con una fonte dati OLE DB o ODBC.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione.

Vedi [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.CredentialsMethodType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione.

Vedi [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getEditPage() {#getEditPage--}
```
public String getEditPage()
```


L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato a fare riferimento a un file XML. In tal caso la pagina destinata all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati in background.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà WebQueryConnection.EditWebPage. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String
### getEditWebPage() {#getEditWebPage--}
```
public String getEditWebPage()
```


L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato a fare riferimento a un file XML. In tal caso la pagina destinata all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati in background.

**Returns:**
java.lang.String
### getHtmlFormat() {#getHtmlFormat--}
```
public int getHtmlFormat()
```


Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True.

Vedi [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Restituisce l'ID della connessione.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


True quando l'applicazione del foglio di calcolo dovrebbe impegnarsi a mantenere la connessione aperta. Quando false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Specifica il nome della connessione. Ogni connessione deve avere un nome univoco.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Specifica il percorso completo al file di connessione esterna da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, l'applicazione del foglio di calcolo proverà di nuovo usando le informazioni dal file di connessione esterna invece dell'oggetto di connessione incorporato nella cartella di lavoro.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Indica se l'applicazione del foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterna indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione del foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Restituisce [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) per una query ODBC o web.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPost() {#getPost--}
```
public String getPost()
```


Restituisce o imposta la stringa utilizzata con il metodo POST per inviare dati a un server web al fine di restituire i dati da una query web.

**Returns:**
java.lang.String
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Restituisce la definizione della formula Power Query.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Specifica cosa dovrebbe fare l'applicazione del foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.

Vedi [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.ReconnectionMethodType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Specifica cosa dovrebbe fare l'applicazione del foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.

Vedi [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


Vero se questa connessione deve essere aggiornata all'apertura del file; altrimenti, falso.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermedio spreadsheetML e la fonte dati esterna.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Vero se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, falso.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


Vero se la password deve essere salvata come parte della stringa di connessione; altrimenti, Falso.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente alcuna clausola WHERE nella prima). Sulla base di questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e possono essere costruite query parametrizzate.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Utilizzato quando la fonte dati esterna è basata su file. Quando una connessione a tale fonte dati fallisce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espresso in notazione URI o percorso file specifico del sistema.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Ottiene il tipo di DataSource della connessione esterna.

Vedi [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di DataSource della connessione esterna.

Vedi [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.SourceType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getUrl() {#getUrl--}
```
public String getUrl()
```


URL da utilizzare per aggiornare i dati esterni.

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


Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indica se la connessione del workbook associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false.

**Returns:**
boolean
### isHtmlTables() {#isHtmlTables--}
```
public boolean isHtmlTables()
```


Flag che indica se le query web devono funzionare solo su tabelle HTML.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno.

**Returns:**
boolean
### isParsePre() {#isParsePre--}
```
public boolean isParsePre()
```


Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query.

**Returns:**
boolean
### isSameSettings() {#isSameSettings--}
```
public boolean isSameSettings()
```


Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga.

**Returns:**
boolean
### isTextDates() {#isTextDates--}
```
public boolean isTextDates()
```


Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date.

**Returns:**
boolean
### isXl2000() {#isXl2000--}
```
public boolean isXl2000()
```


Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato.

**Returns:**
boolean
### isXl97() {#isXl97--}
```
public boolean isXl97()
```


Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato.

**Returns:**
boolean
### isXml() {#isXml--}
```
public boolean isXml()
```


true se la sorgente della query web è XML (invece di HTML), altrimenti false.

**Returns:**
boolean
### isXmlSourceData() {#isXmlSourceData--}
```
public boolean isXmlSourceData()
```


Flag che indica che i dati sorgente XML dovrebbero essere importati invece della tabella HTML stessa.

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


Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronamente in background; false se l'uso preferito della connessione è aggiornare sincronicamente in primo piano.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


La stringa contenente il comando del database da passare all'API del provider di dati che interagirà con la fonte esterna per recuperare i dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Specifica il tipo di comando OLE DB. 1. La query specifica un nome di cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome di tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è rivolta a un provider di dati elenco basato sul web.

Vedi [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Specifica la descrizione dell'utente per questa connessione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


La stringa di informazioni sulla connessione è utilizzata per stabilire un contatto con una fonte dati OLE DB o ODBC.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setConsecutive(boolean value) {#setConsecutive-boolean-}
```
public void setConsecutive(boolean value)
```


Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione.

Vedi [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.CredentialsMethodType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Specifica il metodo di autenticazione da utilizzare durante la creazione (o la ricreazione) della connessione.

Vedi [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indica se la connessione del workbook associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEditPage(String value) {#setEditPage-java.lang.String-}
```
public void setEditPage(String value)
```


L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato a fare riferimento a un file XML. In tal caso la pagina destinata all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati in background.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà WebQueryConnection.EditWebPage. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setEditWebPage(String value) {#setEditWebPage-java.lang.String-}
```
public void setEditWebPage(String value)
```


L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato a fare riferimento a un file XML. In tal caso la pagina destinata all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati in background.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setHtmlFormat(int value) {#setHtmlFormat-int-}
```
public void setHtmlFormat(int value)
```


Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True.

Vedi [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHtmlTables(boolean value) {#setHtmlTables-boolean-}
```
public void setHtmlTables(boolean value)
```


Flag che indica se le query web devono funzionare solo su tabelle HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


True quando l'applicazione del foglio di calcolo dovrebbe impegnarsi a mantenere la connessione aperta. Quando false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Specifica il nome della connessione. Ogni connessione deve avere un nome univoco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Specifica il percorso completo al file di connessione esterna da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, l'applicazione del foglio di calcolo proverà di nuovo usando le informazioni dal file di connessione esterna invece dell'oggetto di connessione incorporato nella cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Indica se l'applicazione del foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterna indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione del foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setParsePre(boolean value) {#setParsePre-boolean-}
```
public void setParsePre(boolean value)
```


Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPost(String value) {#setPost-java.lang.String-}
```
public void setPost(String value)
```


Restituisce o imposta la stringa utilizzata con il metodo POST per inviare dati a un server web al fine di restituire i dati da una query web.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Specifica cosa dovrebbe fare l'applicazione del foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.

Vedi [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.ReconnectionMethodType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Specifica cosa dovrebbe fare l'applicazione del foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.

Vedi [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


Vero se questa connessione deve essere aggiornata all'apertura del file; altrimenti, falso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermedio spreadsheetML e la fonte dati esterna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSameSettings(boolean value) {#setSameSettings-boolean-}
```
public void setSameSettings(boolean value)
```


Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Vero se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, falso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


Vero se la password deve essere salvata come parte della stringa di connessione; altrimenti, Falso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente alcuna clausola WHERE nella prima). Sulla base di questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e possono essere costruite query parametrizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Utilizzato quando la fonte dati esterna è basata su file. Quando una connessione a tale fonte dati fallisce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espresso in notazione URI o percorso file specifico del sistema.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Imposta il tipo di DataSource della connessione esterna.

Vedi [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextDates(boolean value) {#setTextDates-boolean-}
```
public void setTextDates(boolean value)
```


Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta il tipo di DataSource della connessione esterna.

Vedi [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.SourceType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUrl(String value) {#setUrl-java.lang.String-}
```
public void setUrl(String value)
```


URL da utilizzare per aggiornare i dati esterni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setXl2000(boolean value) {#setXl2000-boolean-}
```
public void setXl2000(boolean value)
```


Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setXl97(boolean value) {#setXl97-boolean-}
```
public void setXl97(boolean value)
```


Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostata su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setXml(boolean value) {#setXml-boolean-}
```
public void setXml(boolean value)
```


true se la sorgente della query web è XML (invece di HTML), altrimenti false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setXmlSourceData(boolean value) {#setXmlSourceData-boolean-}
```
public void setXmlSourceData(boolean value)
```


Flag che indica che i dati sorgente XML dovrebbero essere importati invece della tabella HTML stessa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

