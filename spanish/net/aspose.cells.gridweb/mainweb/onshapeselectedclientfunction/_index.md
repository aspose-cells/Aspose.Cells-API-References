---
title: OnShapeSelectedClientFunction
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así función MyOnSelectShapeforma  var nombreforma.getAttributenombrevalor var textshape.getAttributetextvalue var valorforma.getAttributevalor de control var tipoforma.getAttributemsotype  Nota puede usar el puntero este en la función del cliente para señalar el control de cuadrícula que activa el evento.
type: docs
weight: 690
url: /es/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así: función MyOnSelectShape(forma) { var nombre=forma.getAttribute("nombrevalor") var text=shape.getAttribute("textvalue") var valor=forma.getAttribute("valor de control") var tipo=forma.getAttribute("msotype") } Nota: puede usar el puntero "este" en la función del cliente para señalar el control de cuadrícula que activa el evento.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### Ver también

* class [MainWeb](../../mainweb)
* espacio de nombres [Aspose.Cells.GridWeb](../../mainweb)
* asamblea [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
