---
title: classe ConnectionParameter
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 10
url: /it/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  classe ConnectionParameter
Specifica le proprietà relative a qualsiasi parametro utilizzato con le connessioni dati esterne
I parametri sono validi per query ODBC e Web.



Il tipo ConnectionParameter espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [sql_type](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | Tipo di dati SQL del parametro. Valido solo per le origini ODBC.|
| [refresh_on_change](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Flag che indica se la query deve essere aggiornata automaticamente quando il contenuto di a<br/> cella che fornisce le modifiche al valore del parametro. Se vero, i dati esterni vengono aggiornati<br/> utilizzando il nuovo valore del parametro ogni volta che c'è una modifica.<br/> viene aggiornato solo quando richiesto dall'utente o qualche altro evento attiva l'aggiornamento (ad esempio, cartella di lavoro aperta).|
| [prompt](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Stringa di richiesta per il parametro. Presentato all'utente del foglio di lavoro insieme all'interfaccia utente di input<br/> per raccogliere il valore del parametro prima di aggiornare i dati esterni.<br/>parameterType = prompt.|
| [type](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/type) | Tipo di parametro utilizzato.<br/> Se parameterType=value, il valore da boolean, double, integer,<br/> o verrà utilizzata una stringa.<br/> Verrà specificato {boolean, double, integer o string}.|
| [name](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/name) | Il nome del parametro.|
| [cell_reference](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell riferimento che indica il valore della cella da utilizzare per il parametro della query Utilizzato solo quando parameterType è cell.|
| [value](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/value) | Valore numerico non intero, valore intero, valore stringa o valore booleano<br/> da utilizzare come parametro di query.|



###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
