---
title: CustomCommandButtonCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la colección de CustomCommandButton.
type: docs
weight: 60
url: /es/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

Representa la colección de CustomCommandButton.

```csharp
public class CustomCommandButtonCollection : IList
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count) { get; } | Obtiene el recuento de la colección. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize) { get; } | Solo uso interno. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly) { get; } | Solo uso interno. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized) { get; } | Solo uso interno. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item) { get; set; } | Obtiene un objeto de botón de comando personalizado en el índice. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot) { get; } | Solo uso interno. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add)(object) | Agregue un objeto de botón de comando personalizado a la colección. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear)() | Borra la colección. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains)(object) | Indica si el objeto de botón de comando personalizado está en la colección. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto)(Array, int) | Copia la colección a una matriz. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator)() | Obtiene un objeto IEnumerator de la colección. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof)(object) | Obtiene el índice del botón. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert)(int, object) | Inserta un botón en el índice. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove)(object) | Elimina el objeto de botón de comando personalizado. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat)(int) | Elimina en el índice. |

### Ejemplos

```csharp
[C#]
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### Ver también

* espacio de nombres [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
