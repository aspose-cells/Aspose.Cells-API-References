---
title: "FormatConditionCollection Classe"
linktitle: "FormatConditionCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "FormatConditionCollection classe. Incapsula l'oggetto che rappresenta formatconditioncollection in Go."
type: docs
weight: 200
url: /it/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Rappresenta la formattazione condizionale.I FormatConditions possono contenere fino a tre formati condizionali.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | Aggiunge una condizione di formattazione e l'intervallo di celle interessato a FormatConditionsThe FormatConditions può contenere fino a tre conditional formats.Riferimenti ad altri fogli non sono consentiti nelle formule della conditional formatting. |
| [AddArea](./addarea/) | Aggiunge un intervallo di celle formattato condizionalmente. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Aggiunge una condizione di formattazione. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Aggiungi una condizione di formato. |
| [GetCount](./getcount/) | Restituisce il conteggio delle condizioni. |
| [GetRangeCount](./getrangecount/) | Restituisce il conteggio degli intervalli formattati condizionalmente. |
| [Get](./get/) | Restituisce la condizione di formattazione per indice. |
| [GetCellArea](./getcellarea/) | Restituisce l'intervallo di celle formattato condizionalmente per indice. |
| [RemoveArea_Int](./removearea_int/) | Rimuove l'intervallo di celle formattato condizionalmente per indice. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Rimuovi conditional formatting nell'intervallo. |
| [RemoveCondition](./removecondition/) | Rimuove la condizione di formattazione per indice. |
