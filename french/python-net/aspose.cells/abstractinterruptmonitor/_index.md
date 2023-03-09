---
title: AbstractInterruptMonitor classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor classe
Surveillez les demandes interrompues dans toutes les opérations chronophages.



Le type AbstractInterruptMonitor expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_interruption_requested](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Indique si une interruption est demandée pour l'opération en cours.<br/>Si vrai, l'opération en cours sera interrompue.<br/>La mise en œuvre doit effectuer une vérification rapide et efficace ici, sinon cela peut devenir un autre goulot d'étranglement pour la procédure.|
| [terminate_without_exception](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | Lorsque la procédure est interrompue, s'il faut terminer la procédure silencieusement ou lever une exception.<br/>La valeur par défaut est false, c'est-à-dire que lorsque [AbstractInterruptMonitor.is_interruption_requested](/cells/fr/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) est vrai,<br/> un [CellsException](/cells/fr/python-net/aspose.cells/cellsexception) avec le code [ExceptionType.INTERRUPTED](/cells/fr/python-net/aspose.cells/exceptiontype#INTERRUPTED) sera lancé.|



###  Voir également
* module [aspose.cells](..)
* classe [CellsException](/cells/fr/python-net/aspose.cells/cellsexception)
