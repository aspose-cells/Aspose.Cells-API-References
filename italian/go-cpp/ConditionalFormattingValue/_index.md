---
title: "ConditionalFormattingValue Classe"
linktitle: "ConditionalFormattingValue"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "ConditionalFormattingValue classe. Incapsula l'oggetto che rappresenta conditionalformattingvalue in Go."
type: docs
weight: 200
url: /it/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Descrive i valori dei punti di interpolazione in una scala gradiente, dataBar o iconSet.

```go

type ConditionalFormattingValue struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetValue](./getvalue/) | Ottieni o imposta il valore di questo oggetto di valore di formattazione condizionale. Dovrebbe essere usato in congiunzione con Type. |
| [SetValue](./setvalue/) | Ottieni o imposta il valore di questo oggetto di valore di formattazione condizionale. Dovrebbe essere usato in congiunzione con Type. |
| [GetType](./gettype/) | Ottieni o imposta il tipo di questo oggetto di valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente \"Value\" a null. |
| [SetType](./settype/) | Ottieni o imposta il tipo di questo oggetto di valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente \"Value\" a null. |
| [IsGTE](./isgte/) | Ottieni o imposta il flag Maggiore o Uguale. Usa solo per set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. 'false' indica che viene usato 'maggiore' invece di 'maggiore o uguale'. Il valore predefinito è true. |
| [SetIsGTE](./setisgte/) | Ottieni o imposta il flag Maggiore o Uguale. Usa solo per set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. 'false' indica che viene usato 'maggiore' invece di 'maggiore o uguale'. Il valore predefinito è true. |
