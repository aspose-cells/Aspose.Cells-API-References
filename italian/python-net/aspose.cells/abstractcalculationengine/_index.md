---
title: classe AbstractCalculationEngine
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  classe AbstractCalculationEngine
Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.



Il tipo AbstractCalculationEngine espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_param_literal_required](/cells/it/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Indica se questo motore necessita del testo letterale del parametro durante l'esecuzione del calcolo. Il valore predefinito è falso.|
| [process_built_in_functions](/cells/it/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Se le funzioni integrate che sono state supportate dal motore integrato devono essere verificate ed elaborate da questa implementazione.<br/>L'impostazione predefinita è false.<br/> Se l'utente deve modificare la logica di calcolo di alcune funzioni integrate, questa proprietà deve essere impostata su true.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [calculate(data)](/cells/it/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Calcola una funzione con dati dati.|



###  Osservazioni

L'utente non deve modificare alcuna parte della cartella di lavoro direttamente in questa implementazione (tranne il risultato calcolato della funzione personalizzata, che può essere impostata dalla proprietà CalculationData.CalculatedValue).
In caso contrario, potrebbero verificarsi risultati imprevisti o eccezioni.
Se l'utente deve modificare altri dati rispetto al risultato calcolato nell'implementazione di alcune funzioni personalizzate,
ad esempio, modificare la formula della cella, lo stile, ... ecc., l'utente deve raccogliere tali dati in questa implementazione e modificarli al di fuori dell'ambito del calcolo della formula.

###  Guarda anche
* modulo [aspose.cells](..)
