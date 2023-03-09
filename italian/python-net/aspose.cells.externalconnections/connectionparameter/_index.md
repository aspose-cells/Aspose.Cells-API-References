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
I parametri sono validi per query ODBC e web.



Il tipo ConnectionParameter espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [sql_type](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | Tipo di dati SQL del parametro. Valido solo per sorgenti ODBC.|
| [refresh_on_change](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Flag che indica se la query deve essere aggiornata automaticamente quando il contenuto di a<br/> cella che fornisce le modifiche al valore del parametro. Se true, i dati esterni vengono aggiornati<br/> utilizzando il nuovo valore del parametro ogni volta che c'è una modifica. Se falso, dati esterni<br/> viene aggiornato solo quando richiesto dall'utente o qualche altro evento attiva l'aggiornamento (ad esempio, cartella di lavoro aperta).|
| [prompt](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Stringa di prompt per il parametro. Presentato all'utente del foglio di calcolo insieme all'interfaccia utente di input<br/> per raccogliere il valore del parametro prima di aggiornare i dati esterni. Usato solo quando<br/> parameterType = prompt.|
| [type](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/type) | Tipo di parametro utilizzato.<br/>Se parameterType=value, il valore da boolean, double, integer,<br/> o verrà utilizzata una stringa. In questo caso, è previsto che solo uno di<br/> Verrà specificato {boolean, double, integer o string}.|
| [name](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/name) | Il nome del parametro.|
| [cell_reference](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell riferimento che indica il valore della cella da utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell.|
| [value](/cells/it/python-net/aspose.cells.externalconnections/connectionparameter/value) |Valore numerico non intero, valore intero, valore stringa o valore booleano<br/> da utilizzare come parametro di query. Utilizzato solo quando parameterType è value.|



###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
