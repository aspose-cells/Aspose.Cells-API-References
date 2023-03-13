---
title: InterruptMonitor Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 950
url: /de/python-net/aspose.cells/interruptmonitor/
is_root: false
---
##  InterruptMonitor Klasse
Stellt alle Operatoren über den Interrupt dar.



**Nachlass:** [InterruptMonitor](/cells/python-net/aspose.cells/interruptmonitor) → 
[AbstractInterruptMonitor](/cells/de/python-net/aspose.cells/abstractinterruptmonitor)



Der Typ InterruptMonitor macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [InterruptMonitor()](/cells/de/python-net/aspose.cells/interruptmonitor/__init__/#) | Erstellt eine neue Instanz von InterruptMonitor|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_interruption_requested](/cells/de/python-net/aspose.cells/interruptmonitor/is_interruption_requested) | Markieren Sie den Monitor als Unterbrechung anfordernd|
| [terminate_without_exception](/cells/de/python-net/aspose.cells/interruptmonitor/terminate_without_exception) | Wenn die Prozedur unterbrochen wird, ob die Prozedur stillschweigend beendet oder eine Ausnahme ausgelöst wird.<br/>Standard ist falsch, das heißt, wenn [AbstractInterruptMonitor.is_interruption_requested](/cells/de/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) wahr ist,<br/> ein [CellsException](/cells/de/python-net/aspose.cells/cellsexception) mit dem Code [ExceptionType.INTERRUPTED](/cells/de/python-net/aspose.cells/exceptiontype#INTERRUPTED) wird geworfen.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [interrupt()](/cells/de/python-net/aspose.cells/interruptmonitor/interrupt/#) | Unterbrechen Sie den aktuellen Operator.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [AbstractInterruptMonitor](/cells/de/python-net/aspose.cells/abstractinterruptmonitor)
* Klasse [CellsException](/cells/de/python-net/aspose.cells/cellsexception)
* Klasse [InterruptMonitor](/cells/de/python-net/aspose.cells/interruptmonitor)
