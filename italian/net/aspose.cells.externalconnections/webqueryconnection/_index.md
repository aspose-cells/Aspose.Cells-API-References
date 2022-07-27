---
title: WebQueryConnection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Specifica le proprietà per unorigine query Web. Una query Web recupererà i dati dalle tabelle HTML e può anche fornire parametri HTTP Get che devono essere elaborati dal server Web nella generazione dellHTML da inclusi i parametri e gli elementi dei parametri.
type: docs
weight: 3350
url: /it/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Specifica le proprietà per un'origine query Web. Una query Web recupererà i dati dalle tabelle HTML, e può anche fornire parametri HTTP "Get" che devono essere elaborati dal server Web nella generazione dell'HTML da inclusi i parametri e gli elementi dei parametri.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indica se la connessione può essere aggiornata in background (in modo asincrono). true se l'utilizzo preferito della connessione prevede l'aggiornamento asincrono in background; false se l'utilizzo preferito della connessione prevede l'aggiornamento sincrono in primo piano. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Specifica la descrizione utente per questa connessione |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Specifica l'identificatore univoco di questa connessione. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Specifica il metodo di autenticazione da utilizzare per stabilire (o ristabilire) la connessione. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | L'URL della pagina Web rivolta all'utente che mostra i dati della query Web. Questo URL è persistente nel caso in cui sourceData="true" e url siano stati reindirizzati per fare riferimento a un file XML. Quindi la pagina rivolta all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati dietro le quinte. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | Come gestire la formattazione dall'origine HTML quando si importano dati di query Web nel foglio di lavoro . Rilevante quando sourceData è True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Ottiene l'ID della connessione. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | Flag che indica se i delimitatori consecutivi devono essere trattati come un solo delimitatore. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indica se la connessione alla cartella di lavoro associata è stata eliminata. true se la connessione è stata eliminata; in caso contrario, falso. |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | Flag che indica se le query web devono funzionare solo su tabelle HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True se la connessione non è stata aggiornata per la prima volta; altrimenti falso. Questo stato può verificarsi quando l'utente salva il file prima che una query sia terminata. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | Flag che indica se i dati contenuti nei tag HTML PRE nella pagina Web vengono analizzati in colonne quando si importa la pagina in una tabella di query. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | Contrassegno che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | Questo flag esiste per la compatibilità con le versioni precedenti con file di fogli di calcolo esistenti precedenti ed è impostato su true se questa query Web è stata aggiornata in un'applicazione per fogli di calcolo più recente o uguale a a Microsoft Excel 2000. Questo è un attributo facoltativo che può essere ignorato. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | Questo flag esiste per la compatibilità con le versioni precedenti con i file di foglio di calcolo esistenti precedenti ed è impostato su true se questa query Web è stata creata in Microsoft Excel 97. Questo è un attributo facoltativo che può essere ignorato. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | true se l'origine della query Web è XML (rispetto a HTML), altrimenti false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | Flag che indica che i dati di origine XML devono essere importati invece della tabella HTML stessa. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Vero quando l'applicazione del foglio di calcolo dovrebbe tentare di mantenere aperta la connessione . Se false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Specifica il percorso completo del file di connessione esterno da cui è stata creata questa connessione . Se una connessione non riesce durante un tentativo di aggiornamento dei dati e reconnectionMethod=1, , l'applicazione del foglio di calcolo tenterà di nuovo utilizzando le informazioni dal file di connessione esterno invece dell'oggetto di connessione incorporato nella cartella di lavoro. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indica se l'applicazione del foglio di calcolo deve utilizzare sempre e solo le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione del foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Ottiene[`ConnectionParameterCollection`](../connectionparametercollection) per una query ODBC o Web. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | Restituisce o imposta la stringa utilizzata con il metodo post per l'immissione di dati in un server Web per restituire i dati da una query Web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Ottiene la definizione della formula della query di alimentazione. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione non riesce. Il valore predefinito è ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True se questa connessione deve essere aggiornata all'apertura del file; in caso contrario, falso. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti falso. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True se la password deve essere salvata come parte della stringa di connessione; in caso contrario, Falso. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Utilizzato quando l'origine dati esterna è basata su file. Quando una connessione a tale origine dati non riesce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espresso nell'URI o nella notazione del percorso del file specifica del sistema. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server spreadsheetML intermedio e l'origine dati esterna. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Ottiene o imposta il tipo DataSource della connessione esterna. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | URL da utilizzare per aggiornare i dati esterni. |

### Guarda anche

* class [ExternalConnection](../externalconnection)
* spazio dei nomi [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
