---
title: CalculationPrecisionStrategy enumerazione
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1820
url: /it/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
##  CalculationPrecisionStrategy enumerazione
Enumera le strategie per la gestione della precisione di calcolo.
A causa del problema di precisione dell'aritmetica in virgola mobile IEEE 754, alcune formule "apparentemente semplici" potrebbero non essere calcolate come risultato previsto.
Come la formula "=-0.45+0.43+0.02", quando si calcolano direttamente gli operandi con l'operatore '+', il risultato non è zero. Per questo tipo di problema di precisione,
alcune strategie speciali possono dare il risultato atteso.



Il tipo CalculationPrecisionStrategy espone i membri seguenti:

###  Campi
| Campo| Descrizione|
| :- | :- |
| NONE | Nessuna strategia applicata al calcolo.<br/>Durante il calcolo basta usare il valore double originale come operando e restituire direttamente il risultato.<br/> Più efficiente per le prestazioni e applicabile per la maggior parte dei casi.|
| ROUND | Arrotonda il risultato del calcolo in base alle cifre significative.|
| DECIMAL | Usa i decimali come operandi quando possibile.<br/> Più inefficiente per le prestazioni.|



###  Guarda anche
* modulo [aspose.cells](..)
