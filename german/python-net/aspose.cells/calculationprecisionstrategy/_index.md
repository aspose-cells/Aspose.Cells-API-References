---
title: CalculationPrecisionStrategy Aufzählung
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1820
url: /de/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
##  CalculationPrecisionStrategy Aufzählung
Listet Strategien zum Umgang mit der Berechnungsgenauigkeit auf.
Aufgrund des Genauigkeitsproblems der IEEE 754-Gleitkommaarithmetik werden einige "scheinbar einfache" Formeln möglicherweise nicht als erwartetes Ergebnis berechnet.
Wie Formel "=-0,45+0,43+0,02", wenn Operanden direkt mit dem Operator "+" berechnet werden, ist das Ergebnis nicht Null. Für solche Präzisionsprobleme
Einige spezielle Strategien können das erwartete Ergebnis liefern.



Der Typ CalculationPrecisionStrategy macht die folgenden Member verfügbar:

###  Felder
| Feld| Beschreibung|
| :- | :- |
| NONE | Bei der Berechnung wurde keine Strategie angewendet.<br/>Verwenden Sie bei der Berechnung einfach den ursprünglichen Double-Wert als Operanden und geben Sie das Ergebnis direkt zurück.<br/> Am effizientesten für die Leistung und für die meisten Fälle geeignet.|
| ROUND | Rundet das Rechenergebnis nach signifikanten Stellen.|
| DECIMAL | Verwendet nach Möglichkeit Dezimalzahlen als Operanden.<br/> Am ineffizientesten für die Leistung.|



###  Siehe auch
* Modul [aspose.cells](..)
