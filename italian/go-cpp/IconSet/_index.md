---
title: "IconSet Classe"
linktitle: "IconSet"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "IconSet class. Incapsula l'oggetto che rappresenta iconset in Go."
type: docs
weight: 200
url: /it/go-cpp/iconset/
---

## IconSet class

Descrive la regola di formattazione condizionale IconSet.Questa regola di formattazione condizionale applica icone alle celle secondo i loro valori.

```go

type IconSet struct  {
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
| [GetCfIcons](./getcficons/) | Ottieni theConditionalFormattingIcon dalla collezione |
| [GetCfvos](./getcfvos/) | Ottieni l'istanza di CFValueObjects. |
| [GetType](./gettype/) | Ottieni o imposta il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente di Cfvos è conforme al nuovo tipo. Se non è conforme, i vecchi Cfvos verranno puliti e verranno aggiunti i Cfvos predefiniti. |
| [SetType](./settype/) | Ottieni o imposta il tipo di set di icone da visualizzare. Impostare il tipo verificherà automaticamente se il conteggio corrente di Cfvos è conforme al nuovo tipo. Se non è conforme, i vecchi Cfvos verranno puliti e verranno aggiunti i Cfvos predefiniti. |
| [IsCustom](./iscustom/) | Indica se il set di icone è personalizzato. Il valore predefinito è false. |
| [GetShowValue](./getshowvalue/) | Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. Il valore predefinito è true. |
| [SetShowValue](./setshowvalue/) | Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicato questo set di icone. Il valore predefinito è true. |
| [GetReverse](./getreverse/) | Ottieni o imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false. |
| [SetReverse](./setreverse/) | Ottieni o imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false. |
