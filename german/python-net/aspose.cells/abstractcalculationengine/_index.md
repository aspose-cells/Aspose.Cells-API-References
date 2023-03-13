---
title: AbstractCalculationEngine Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  AbstractCalculationEngine Klasse
Stellt das benutzerdefinierte Berechnungsmodul des Benutzers dar, um das standardmäßige Berechnungsmodul von Aspose.Cells zu erweitern.



Der Typ AbstractCalculationEngine macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_param_literal_required](/cells/de/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Gibt an, ob diese Engine während der Berechnung den wörtlichen Text des Parameters benötigt. Der Standardwert ist falsch.|
| [process_built_in_functions](/cells/de/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Ob eingebaute Funktionen, die von der eingebauten Engine unterstützt wurden, von dieser Implementierung überprüft und verarbeitet werden sollen.<br/>Standard ist falsch.<br/> Wenn der Benutzer die Berechnungslogik einiger integrierter Funktionen ändern muss, sollte diese Eigenschaft auf „true“ gesetzt werden.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [calculate(data)](/cells/de/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Berechnet eine Funktion mit gegebenen Daten.|



###  Bemerkungen

Der Benutzer sollte keinen Teil der Arbeitsmappe direkt in dieser Implementierung ändern (mit Ausnahme des berechneten Ergebnisses der benutzerdefinierten Funktion, das durch die Eigenschaft CalculationData.CalculatedValue festgelegt werden kann).
Andernfalls kann es zu einem unerwarteten Ergebnis oder einer Ausnahme kommen.
Wenn der Benutzer andere Daten als das berechnete Ergebnis in der Implementierung für einige benutzerdefinierte Funktionen ändern muss,
B. die Formel, den Stil usw. der Zelle ändern, sollte der Benutzer diese Daten in dieser Implementierung sammeln und sie aus dem Bereich der Formelberechnung heraus ändern.

###  Siehe auch
* Modul [aspose.cells](..)
