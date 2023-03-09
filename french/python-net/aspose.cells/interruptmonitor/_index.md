---
title: InterruptMonitor classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 950
url: /fr/python-net/aspose.cells/interruptmonitor/
is_root: false
---
##  InterruptMonitor classe
Représente tous les opérateurs concernant l'interruption.



**Héritage:** [InterruptMonitor](/cells/python-net/aspose.cells/interruptmonitor) → 
[AbstractInterruptMonitor](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor)



Le type InterruptMonitor expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [InterruptMonitor()](/cells/fr/python-net/aspose.cells/interruptmonitor/__init__/#) | Construit une nouvelle instance d'InterruptMonitor|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_interruption_requested](/cells/fr/python-net/aspose.cells/interruptmonitor/is_interruption_requested) | Marquer le moniteur comme demandant une interruption|
| [terminate_without_exception](/cells/fr/python-net/aspose.cells/interruptmonitor/terminate_without_exception) | Lorsque la procédure est interrompue, s'il faut terminer la procédure silencieusement ou lever une exception.<br/>La valeur par défaut est false, c'est-à-dire que lorsque [AbstractInterruptMonitor.is_interruption_requested](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) est vrai,<br/> un [CellsException](/cells/fr/python-net/aspose.cells/cellsexception) avec le code [ExceptionType.INTERRUPTED](/cells/fr/python-net/aspose.cells/exceptiontype#INTERRUPTED) sera lancé.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [interrupt()](/cells/fr/python-net/aspose.cells/interruptmonitor/interrupt/#) | Interrompre l'opérateur en cours.|



###  Voir également
* module [aspose.cells](..)
* classe [AbstractInterruptMonitor](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor)
* classe [CellsException](/cells/fr/python-net/aspose.cells/cellsexception)
* classe [InterruptMonitor](/cells/fr/python-net/aspose.cells/interruptmonitor)
