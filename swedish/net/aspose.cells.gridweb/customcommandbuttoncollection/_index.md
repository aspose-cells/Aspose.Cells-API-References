---
title: "Klass CustomCommandButtonCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.CustomCommandButtonCollection-klass. Representerar samlingen av CustomCommandButton"
type: docs
url: /sv/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

Representerar samlingen av CustomCommandButton.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | Hämtar antalet i samlingen. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | Endast för internt bruk. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | Endast för internt bruk. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | Endast för internt bruk. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | Hämtar ett anpassat kommandoknappobjekt på indexet. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | Endast för internt bruk. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | Lägg till ett anpassat kommandoknappobjekt i samlingen. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | Rensar samlingen. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | Anger om det anpassade kommandoknappobjektet finns i samlingen. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | Kopierar samlingen till en array. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | Hämtar ett IEnumerator-objekt från samlingen. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | Hämtar indexet för knappen. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | Infogar en knapp på indexet. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | Tar bort det anpassade kommandoknappobjektet. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | Tar bort på indexet. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


