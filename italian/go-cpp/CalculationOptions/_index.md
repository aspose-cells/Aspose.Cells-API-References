---
title: "Classe CalculationOptions"
linktitle: "CalculationOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe CalculationOptions. Incapsula l'oggetto che rappresenta calculationoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/calculationoptions/
---

## CalculationOptions class

Rappresenta le opzioni per il calcolo.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetIgnoreError](./getignoreerror/) | Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati.L'errore può essere una funzione non supportata, collegamenti esterni, ecc.Il valore predefinito è vero. |
| [SetIgnoreError](./setignoreerror/) | Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati.L'errore può essere una funzione non supportata, collegamenti esterni, ecc.Il valore predefinito è vero. |
| [GetRecursive](./getrecursive/) | Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle.Il valore predefinito è vero. |
| [SetRecursive](./setrecursive/) | Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle.Il valore predefinito è vero. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Indica se l'utente ha specificato esplicitamente il comportamento di aggiornamento delle formule di array dinamici prima di calcolare le formule specificate. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule. |
| [GetCustomEngine](./getcustomengine/) | Il motore di calcolo delle formule personalizzato per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [SetCustomEngine](./setcustomengine/) | Il motore di calcolo delle formule personalizzato per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [GetCalcStackSize](./getcalcstacksize/) | La dimensione dello stack per calcolare le celle ricorsivamente. Il valore predefinito è 200. |
| [SetCalcStackSize](./setcalcstacksize/) | La dimensione dello stack per calcolare le celle ricorsivamente. Il valore predefinito è 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | Specifica la strategia per l'elaborazione della precisione del calcolo. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | Specifica la strategia per l'elaborazione della precisione del calcolo. |
| [GetLinkedDataSources](./getlinkeddatasources/) | Specifica le origini dati per i collegamenti esterni utilizzati nelle formule. |
| [SetLinkedDataSources](./setlinkeddatasources/) | Specifica le origini dati per i collegamenti esterni utilizzati nelle formule. |
| [GetCharacterEncoding](./getcharacterencoding/) | Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR, CODE, il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da utilizzare per tali funzioni per ottenere il risultato previsto. |
| [SetCharacterEncoding](./setcharacterencoding/) | Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR, CODE, il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da utilizzare per tali funzioni per ottenere il risultato previsto. |
