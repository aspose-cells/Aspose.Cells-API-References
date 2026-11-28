---
title: "Sınıf CustomCommandButtonCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.CustomCommandButtonCollection sınıfı. CustomCommandButton koleksiyonunu temsil eder."
type: docs
url: /tr/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

CustomCommandButton koleksiyonunu temsil eder.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | Koleksiyonun sayısını alır. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | Sadece dahili kullanım için. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | Sadece dahili kullanım için. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | Sadece dahili kullanım için. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | Belirtilen indekste bir özel komut düğmesi nesnesi alır. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | Sadece dahili kullanım için. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | Koleksiyona bir özel komut düğmesi nesnesi ekle. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | Koleksiyonu temizler. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | Özel komut düğmesi nesnesinin koleksiyonda olup olmadığını gösterir. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | Koleksiyonu bir diziye kopyalar. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | Koleksiyonun bir IEnumerator nesnesini alır. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | Düğmenin indeksini alır. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | İndekste bir düğme ekler. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | Özel komut düğmesi nesnesini kaldırır. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | İndeksten kaldırır. |

### Örnekler

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


