---
title: "MainWeb.OnSubmitClientFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MainWeb property. Ottiene o imposta la funzione client da chiamare prima che il controllo venga inviato lato client. La funzione client dovrebbe essere dichiarata così function MyOnSubmitarg cancelEdit  return true L'arg è l'argomento di submit che contiene il comando da inviare al server. cancelEdit è un valore booleano che indica se il controllo ha scartato l'input dell'utente prima dell'invio. Il controllo continuerà a inviare se la funzione restituisce true. Nota È possibile utilizzare il puntatore this nella funzione client per fare riferimento al controllo grid che genera l'evento"
type: docs
url: /it/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

Ottiene o imposta la funzione client da chiamare prima che il controllo sia inviato lato client. La funzione client dovrebbe essere dichiarata così: function MyOnSubmit(arg, cancelEdit) { return true;} L'arg è l'argomento di invio, contiene il comando da postare al server. Il cancelEdit è un valore booleano che indica se il controllo ha scartato l'input dell'utente prima dell'invio. Il controllo continuerà a inviare se la funzione restituisce true. Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### Vedi anche

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


