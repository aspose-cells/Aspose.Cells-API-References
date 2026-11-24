---
title: "Klasse CustomCommandButtonCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.CustomCommandButtonCollection Klasse. Stellt die Sammlung von CustomCommandButton dar."
type: docs
url: /de/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

Stellt die Sammlung von CustomCommandButton dar.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | Gibt die Anzahl der Sammlung zurück. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | Nur intern verwendet. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | Nur intern verwendet. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | Nur intern verwendet. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | Liefert ein CustomCommandButton-Objekt am Index. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | Nur intern verwendet. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | Fügt ein CustomCommandButton-Objekt zur Sammlung hinzu. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | Leert die Sammlung. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | Gibt an, ob das CustomCommandButton-Objekt in der Sammlung enthalten ist. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | Kopiert die Sammlung in ein Array. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | Liefert ein IEnumerator-Objekt der Sammlung. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | Liefert den Index der Schaltfläche. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | Fügt eine Schaltfläche am Index ein. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | Entfernt das CustomCommandButton-Objekt. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | Entfernt am Index. |

### Beispiele

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim GridWeb1 As GridWeb= New GridWeb();
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### Siehe auch

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


