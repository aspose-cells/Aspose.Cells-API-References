---
title: "Classe FormulaParseOptions"
linktitle: "FormulaParseOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe FormulaParseOptions. Incapsula l'oggetto che rappresenta formulaparseoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

Rappresenta le opzioni durante l'analisi della formula.

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetLocaleDependent](./getlocaledependent/) | Indica se la formula è formattata per locale. Il valore predefinito è false. |
| [SetLocaleDependent](./setlocaledependent/) | Indica se la formula è formattata per locale. Il valore predefinito è false. |
| [GetR1C1Style](./getr1c1style/) | Indica se la formula utilizza lo stile di riferimento R1C1. Il valore predefinito è false. |
| [SetR1C1Style](./setr1c1style/) | Indica se la formula utilizza lo stile di riferimento R1C1. Il valore predefinito è false. |
| [GetCheckAddIn](./getcheckaddin/) | Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per funzioni definite dall'utente senza collegamento esterno. Default è true(se la funzione definita dall'utente corrisponde a un componente aggiuntivo nei collegamenti esterni esistenti, allora viene considerata tale componente). |
| [SetCheckAddIn](./setcheckaddin/) | Indica se verificare i componenti aggiuntivi nei collegamenti esterni esistenti della cartella di lavoro corrente per funzioni definite dall'utente senza collegamento esterno. Default è true(se la funzione definita dall'utente corrisponde a un componente aggiuntivo nei collegamenti esterni esistenti, allora viene considerata tale componente). |
| [GetParse](./getparse/) | Indica se analizzare la formula fornita. Default è true. Se è false, la stringa della formula fornita verrà mantenuta così com'è per la cella finché l'utente non chiama altri metodi per analizzarla o i dati della formula analizzata sono richiesti da altre operazioni, come il calcolo delle formule. |
| [SetParse](./setparse/) | Indica se analizzare la formula fornita. Default è true. Se è false, la stringa della formula fornita verrà mantenuta così com'è per la cella finché l'utente non chiama altri metodi per analizzarla o i dati della formula analizzata sono richiesti da altre operazioni, come il calcolo delle formule. |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | Definizione per l'analisi delle funzioni personalizzate. |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | Definizione per l'analisi delle funzioni personalizzate. |
