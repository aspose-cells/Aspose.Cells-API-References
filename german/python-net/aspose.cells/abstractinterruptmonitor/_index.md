---
title: AbstractInterruptMonitor Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor Klasse
Überwachen Sie alle zeitaufwändigen Vorgänge auf unterbrochene Anforderungen.



Der Typ AbstractInterruptMonitor macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_interruption_requested](/cells/de/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Gibt an, ob eine Unterbrechung für den aktuellen Betrieb angefordert wird.<br/>Wenn wahr, wird der aktuelle Vorgang unterbrochen.<br/>Die Umsetzung sollte hier schnell und effizient prüfen, sonst kann es zu einem weiteren Engpass für das Verfahren werden.|
| [terminate_without_exception](/cells/de/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | Wenn die Prozedur unterbrochen wird, ob die Prozedur ruhig beendet oder eine Ausnahme ausgelöst werden soll.<br/>Standard ist falsch, das heißt, wenn [AbstractInterruptMonitor.is_interruption_requested](/cells/de/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) wahr ist,<br/> ein [CellsException](/cells/de/python-net/aspose.cells/cellsexception) mit dem Code [ExceptionType.INTERRUPTED](/cells/de/python-net/aspose.cells/exceptiontype#INTERRUPTED) wird geworfen.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [CellsException](/cells/de/python-net/aspose.cells/cellsexception)
