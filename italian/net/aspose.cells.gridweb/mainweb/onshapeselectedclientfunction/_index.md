---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MainWeb. Ottiene o imposta la funzione client da chiamare quando una forma è selezionata. La funzione client deve essere dichiarata così: function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype Nota: è possibile utilizzare il puntatore this nella funzione client per fare riferimento al controllo grid che genera l'evento"
type: docs
url: /it/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Ottiene o imposta la funzione lato client da chiamare quando una forma è selezionata. La funzione client dovrebbe essere dichiarata così: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### Vedi anche

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


