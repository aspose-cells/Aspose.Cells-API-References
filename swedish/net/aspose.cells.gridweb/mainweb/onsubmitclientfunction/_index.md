---
title: "MainWeb.OnSubmitClientFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MainWeb property. Hämtar eller anger klientfunktionen som ska anropas innan kontrollen skickas in på klientsidan. Klientfunktionen bör deklareras så här function MyOnSubmitarg cancelEdit  return true Arg är inlämningsargumentet som innehåller kommandot som ska postas till servern. cancelEdit är ett booleskt värde som indikerar om kontrollen har förkastat användarens inmatning före inlämning. Kontrollen fortsätter att skicka om funktionen returnerar true. Notera att du kan använda this‑pekaren i klientfunktionen för att referera till rutnätkontrollen som utlöser händelsen"
type: docs
url: /sv/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

Hämtar eller anger klientfunktionen som ska anropas innan kontrollen skickas in på klientsidan. Klientfunktionen bör deklareras så här: function MyOnSubmit(arg, cancelEdit) { return true;} Arg är inlämningsargumentet och innehåller kommandot som ska postas till servern. cancelEdit är ett booleskt värde som indikerar om kontrollen har förkastat användarens inmatning innan inlämning. Kontrollen fortsätter att skicka om funktionen returnerar true. Obs: Du kan använda \"this\"-pekaren i klientfunktionen för att peka på grid‑kontrollen som utlöser händelsen.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### Se även

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


