---
title: ExternalConnection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells.externalconnections/externalconnection/
is_root: false
---
##  ExternalConnection klass
Anger en extern dataanslutning



Typen ExternalConnection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [id](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/id) | Får anslutningens ID.|
| [power_query_formula](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/power_query_formula) | Hämtar definitionen av kraftfrågeformel.|
| [type](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/type) | Hämtar eller ställer in den externa anslutningens DataSource-typ.|
| [source_file](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/source_file) | Används när den externa datakällan är filbaserad. När en anslutning till en sådan data<br/> källan misslyckas försöker kalkylarksprogrammet ansluta direkt till den här filen. Kanske<br/> uttryckt i URI eller systemspecifik filsökvägsnotation.|
| [sso_id](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/sso_id) | Identifierare för enkel inloggning (SSO) som används för autentisering mellan en intermediär<br/> kalkylarkML-server och den externa datakällan.|
| [save_password](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/save_password) | True om lösenordet ska sparas som en del av anslutningssträngen; annars, Falskt.|
| [save_data](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/save_data) | Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas<br/> med arbetsboken; annars falskt.|
| [refresh_on_load](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/refresh_on_load) | Sant om den här anslutningen ska uppdateras när filen öppnas; annars falskt.|
| [reconnection_method_type](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/reconnection_method_type) | Anger vad kalkylarksapplikationen ska göra när en anslutning misslyckas.<br/>Standardvärdet är ReConnectionMethodType.Required.|
| [reconnection_method](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/reconnection_method) | Anger vad kalkylarksapplikationen ska göra när en anslutning misslyckas.<br/>Standardvärdet är ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/only_use_connection_file) | Anger om kalkylbladsapplikationen alltid och bara ska använda<br/> anslutningsinformation i den externa anslutningsfilen som anges av odcFile-attributet<br/> när anslutningen uppdateras. Om falskt, då kalkylarksapplikationen<br/> bör följa proceduren som anges av attributet reconnectionMethod|
| [odc_file](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/odc_file) | Anger den fullständiga sökvägen till den externa anslutningsfilen från vilken anslutningen kom<br/> skapat. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1,<br/> då försöker kalkylarket igen med information från den externa anslutningsfilen<br/> istället för det anslutningsobjekt som är inbäddat i arbetsboken.|
| [is_new](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/is_new) | Sant om anslutningen inte har uppdaterats för första gången; annars falskt.<br/> Detta tillstånd kan inträffa när användaren sparar filen innan en fråga har slutat returnera.|
| [name](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/name) | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn.|
| [keep_alive](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/keep_alive) | Sant när kalkylprogrammet ska anstränga sig för att behålla anslutningen<br/>öppen. När det är falskt bör applikationen stänga anslutningen efter att ha hämtat<br/> information.|
| [refresh_internal](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/refresh_internal) | Anger antalet minuter mellan automatiska uppdateringar av anslutningen.|
| [connection_id](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/connection_id) | Anger den unika identifieraren för denna anslutning.|
| [connection_description](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/connection_description) | Anger användarbeskrivningen för denna anslutning|
| [is_deleted](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/is_deleted) |Indikerar om den associerade arbetsboksanslutningen har tagits bort. sant om<br/> anslutningen har tagits bort; annars falskt.|
| [credentials_method_type](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/credentials_method_type) | Anger den autentiseringsmetod som ska användas när anslutningen upprättas (eller återupprättas).|
| [credentials](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/credentials) | Anger den autentiseringsmetod som ska användas när anslutningen upprättas (eller återupprättas).|
| [background_refresh](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/background_refresh) | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront).<br/>sant om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden;<br/> false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden.|
| [parameters](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection/parameters) | Får [ConnectionParameterCollection](/cells/sv/python-net/aspose.cells.externalconnections/connectionparametercollection) för en ODBC- eller webbfråga.|



###  Se även
* modul [aspose.cells.externalconnections](..)
* klass [ConnectionParameterCollection](/cells/sv/python-net/aspose.cells.externalconnections/connectionparametercollection)
