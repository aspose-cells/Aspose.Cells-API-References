---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MainWeb egenskap. Hämtar eller anger den klientsidiga funktionen som ska anropas när en form väljs. Klientfunktionen bör deklareras så här: function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype. Obs! Du kan använda this‑pekaren i klientfunktionen för att referera till rutnätkontrollen som utlöser händelsen"
type: docs
url: /sv/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Hämtar eller anger klientsidans funktion som ska anropas när en form väljs. Klientfunktionen bör deklareras så här: function MyOnSelectShape(shape) { var name=shape.getAttribute(\"namevalue\") var text=shape.getAttribute(\"textvalue\") var value=shape.getAttribute(\"controlvalue\") var type=shape.getAttribute(\"msotype\") }Obs: Du kan använda \"this\"-pekaren i klientfunktionen för att peka på grid‑kontrollen som utlöser händelsen.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### Se även

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


