---
title: classe AbstractInterruptMonitor
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 50
url: /it/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  classe AbstractInterruptMonitor
Monitora le richieste di interruzione in tutte le operazioni che richiedono tempo.



Il tipo AbstractInterruptMonitor espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_interruption_requested](/cells/it/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Indica se è richiesta l'interruzione per l'operazione in corso.<br/>Se vero, l'operazione corrente verrà interrotta.<br/>L'implementazione dovrebbe eseguire un controllo rapido ed efficiente qui, altrimenti potrebbe diventare un altro collo di bottiglia per la procedura.|
| [terminate_without_exception](/cells/it/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | Quando la procedura viene interrotta, se terminare la procedura in silenzio o lanciare un'eccezione.<br/>L'impostazione predefinita è false, ovvero quando [AbstractInterruptMonitor.is_interruption_requested](/cells/it/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) è vero,<br/> verrà lanciato uno [CellsException](/cells/it/python-net/aspose.cells/cellsexception) con codice [ExceptionType.INTERRUPTED](/cells/it/python-net/aspose.cells/exceptiontype#INTERRUPTED).|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [CellsException](/cells/it/python-net/aspose.cells/cellsexception)
