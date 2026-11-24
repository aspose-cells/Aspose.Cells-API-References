---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb-Eigenschaft. Gibt die clientseitige Funktion an, die aufgerufen wird, wenn eine Form ausgewählt wird, oder legt sie fest. Die clientseitige Funktion sollte wie folgt deklariert werden: function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype Hinweis: Sie können den this‑Zeiger in der clientseitigen Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Form ausgewählt wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### Siehe auch

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


