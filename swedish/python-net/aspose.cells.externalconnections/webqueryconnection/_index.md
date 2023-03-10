---
title: WebQueryConnection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  WebQueryConnection klass
 Anger egenskaperna för en webbfrågekälla. En webbfråga kommer att hämta data från HTML tabeller,
 och kan också tillhandahålla HTTP "Get"-parametrar som ska bearbetas av webbservern för att generera HTML av
inklusive parametrarna och parameterelementen.



**Arv:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection)



Typen WebQueryConnection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [id](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Får anslutningens ID.|
| [power_query_formula](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Hämtar definitionen av kraftfrågeformel.|
| [type](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Hämtar eller ställer in den externa anslutningens DataSource-typ.|
| [source_file](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Används när den externa datakällan är filbaserad. När en anslutning till en sådan data<br/> källan misslyckas försöker kalkylarksprogrammet ansluta direkt till den här filen. Kanske<br/> uttryckt i URI eller systemspecifik filsökvägsnotation.|
| [sso_id](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Identifierare för enkel inloggning (SSO) som används för autentisering mellan en intermediär<br/> kalkylarkML-server och den externa datakällan.|
| [save_password](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) | True om lösenordet ska sparas som en del av anslutningssträngen; annars, Falskt.|
| [save_data](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas<br/> med arbetsboken; annars falskt.|
| [refresh_on_load](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | Sant om den här anslutningen ska uppdateras när filen öppnas; annars falskt.|
| [reconnection_method_type](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Anger vad kalkylarksapplikationen ska göra när en anslutning misslyckas.<br/>Standardvärdet är ReConnectionMethodType.Required.|
| [reconnection_method](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Anger vad kalkylarksapplikationen ska göra när en anslutning misslyckas.<br/>Standardvärdet är ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Anger om kalkylbladsapplikationen alltid och bara ska använda<br/> anslutningsinformation i den externa anslutningsfilen som anges av odcFile-attributet<br/> när anslutningen uppdateras. Om falskt, då kalkylarksapplikationen<br/> bör följa proceduren som anges av attributet reconnectionMethod|
| [odc_file](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Anger den fullständiga sökvägen till den externa anslutningsfilen från vilken anslutningen kom<br/> skapat. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1,<br/> då försöker kalkylarket igen med information från den externa anslutningsfilen<br/> istället för det anslutningsobjekt som är inbäddat i arbetsboken.|
| [is_new](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | Sant om anslutningen inte har uppdaterats för första gången; annars falskt.<br/> Detta tillstånd kan inträffa när användaren sparar filen innan en fråga har slutat returnera.|
| [name](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn.|
| [keep_alive](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | Sant när kalkylprogrammet ska anstränga sig för att behålla anslutningen<br/>öppen. När det är falskt bör applikationen stänga anslutningen efter att ha hämtat<br/> information.|
| [refresh_internal](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Anger antalet minuter mellan automatiska uppdateringar av anslutningen.|
| [connection_id](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Anger den unika identifieraren för denna anslutning.|
| [connection_description](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Anger användarbeskrivningen för denna anslutning|
| [is_deleted](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) |Indikerar om den associerade arbetsboksanslutningen har tagits bort. sant om<br/> anslutningen har tagits bort; annars falskt.|
| [credentials_method_type](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Anger den autentiseringsmetod som ska användas när anslutningen upprättas (eller återupprättas).|
| [credentials](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Anger den autentiseringsmetod som ska användas när anslutningen upprättas (eller återupprättas).|
| [background_refresh](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront).<br/>sant om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden;<br/> false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden.|
| [parameters](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Får [ConnectionParameterCollection](/cells/sv/python-net/aspose.cells.externalconnections/connectionparametercollection) för en ODBC- eller webbfråga.|
| [is_xml](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | sant om webbfrågans källa är XML (mot HTML), annars falskt.|
| [is_xl97](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) |Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylarksfiler och är inställd<br/>till sant om den här webbfrågan skapades i Microsoft Excel 97.<br/> Detta är ett valfritt attribut som kan ignoreras.|
| [is_xl2000](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) |Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylarksfiler och är inställd<br/>till sant om den här webbfrågan har uppdaterats i ett kalkylarksprogram som är nyare än eller lika<br/>till Microsoft Excel 2000.<br/> Detta är ett valfritt attribut som kan ignoreras.|
| [url](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL att använda för att uppdatera extern data.|
| [is_text_dates](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Flagga som anger om datum ska importeras till celler i kalkylbladet som text snarare än datum.|
| [is_xml_source_data](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Flagga som anger att XML-källdata ska importeras istället för själva tabellen HTML.|
| [post](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Returnerar eller ställer in strängen som används med postmetoden för att mata in data till en webbserver<br/> för att returnera data från en webbfråga.|
| [is_parse_pre](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) | Flagga som anger om data som finns i HTML PRE-taggar på webbsidan är<br/> tolkas i kolumner när du importerar sidan till en frågetabell.|
| [is_html_tables](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Flagga som anger om webbfrågor endast ska fungera på HTML-tabeller.|
| [html_format](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | Hur man hanterar formatering från källan HTML när webbfrågedata överförs till<br/> arbetsblad. Relevant när källdata är sant.|
| [is_same_settings](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) |Flagga som anger om alla tabeller i ett PRE-block ska analyseras med samma breddinställningar<br/> som första raden.|
| [edit_web_page](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | Webbadressen till den användarvända webbsidan som visar webbfrågans data. Den här webbadressen finns kvar<br/>i fallet att sourceData="true" och url har omdirigerats för att referera till en XML-fil.<br/>Sedan kan den användarvända sidan visas i användargränssnittet och XML-data kan hämtas<br/> bakom kulisserna.|
| [edit_page](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | Webbadressen till den användarvända webbsidan som visar webbfrågans data. Den här webbadressen finns kvar<br/>i fallet att sourceData="true" och url har omdirigerats för att referera till en XML-fil.<br/>Sedan kan den användarvända sidan visas i användargränssnittet och XML-data kan hämtas<br/> bakom kulisserna.|
| [is_consecutive](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Flagga som anger om på varandra följande avgränsare ska behandlas som bara en avgränsare.|



###  Se även
* modul [aspose.cells.externalconnections](..)
* klass [ConnectionParameterCollection](/cells/sv/python-net/aspose.cells.externalconnections/connectionparametercollection)
* klass [ExternalConnection](/cells/sv/python-net/aspose.cells.externalconnections/externalconnection)
* klass [WebQueryConnection](/cells/sv/python-net/aspose.cells.externalconnections/webqueryconnection)
