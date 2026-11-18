---
title: "Slicer Klass"
linktitle: "Slicer"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Slicer klass. Inkapslar objektet som representerar slicer i Go."
type: docs
weight: 200
url: /sv/go-cpp/slicer/
---

## Slicer class

sammanfattande beskrivning av Slicer View

```go

type Slicer struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetSortOrderType](./getsortordertype/) | Anger typen av sorteringsobjekt. |
| [SetSortOrderType](./setsortordertype/) | Anger typen av sorteringsobjekt. |
| [GetShowMissing](./getshowmissing/) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [SetShowMissing](./setshowmissing/) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Anger om objekt som har tagits bort från datakällan ska visas. |
| [GetShowAllItems](./getshowallitems/) | Anger om alla objekt ska visas även om det inte finns någon data eller de är borttagna. Standardvärdet är true; |
| [SetShowAllItems](./setshowallitems/) | Anger om alla objekt ska visas även om det inte finns någon data eller de är borttagna. Standardvärdet är true; |
| [AddPivotConnection](./addpivotconnection/) | Lägger till PivotTable-anslutning. |
| [RemovePivotConnection](./removepivotconnection/) | Tar bort PivotTable-anslutning. |
| [GetLockedPosition](./getlockedposition/) | Anger om den angivna slicern kan flyttas eller ändras i storlek via användargränssnittet. |
| [SetLockedPosition](./setlockedposition/) | Anger om den angivna slicern kan flyttas eller ändras i storlek via användargränssnittet. |
| [Refresh](./refresh/) | Uppdaterar slicerns objekt från de associerade pivottabellerna. |
| [GetShape](./getshape/) | Returnerar Shape-objektet som är associerat med den angivna slicern. Endast läs. |
| [GetSlicerCache](./getslicercache/) | Returnerar SlicerCache-objektet som är associerat med slicern. Endast läs. |
| [GetWorksheet](./getworksheet/) | Returnerar Worksheet-objektet som innehåller denna slicer. Endast läs. |
| [GetStyleType](./getstyletype/) | Ange typen av inbyggd slicer-stil. Standardtypen är SlicerStyleLight1. |
| [SetStyleType](./setstyletype/) | Ange typen av inbyggd slicer-stil. Standardtypen är SlicerStyleLight1. |
| [GetName](./getname/) | Returnerar eller anger namnet på den angivna slicern |
| [SetName](./setname/) | Returnerar eller anger namnet på den angivna slicern |
| [GetCaption](./getcaption/) | Returnerar eller anger rubriken för den angivna skivkontrollen. |
| [SetCaption](./setcaption/) | Returnerar eller anger rubriken för den angivna skivkontrollen. |
| [GetFirstItemIndex](./getfirstitemindex/) | Anger det nollbaserade indexet för det första skivkontrollelementet. |
| [SetFirstItemIndex](./setfirstitemindex/) | Anger det nollbaserade indexet för det första skivkontrollelementet. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | Ta bort markerade filteretiketter. |
| [ClearFilter](./clearfilter/) | Ta bort filter |
| [GetShowCaption](./getshowcaption/) | Anger om rubriken för skivkontrollen är synlig.Standardvärdet är true |
| [SetShowCaption](./setshowcaption/) | Anger om rubriken för skivkontrollen är synlig.Standardvärdet är true |
| [GetNumberOfColumns](./getnumberofcolumns/) | Returnerar eller anger antalet kolumner i skivkontrollen.Standardvärdet är 1. |
| [SetNumberOfColumns](./setnumberofcolumns/) | Returnerar eller anger antalet kolumner i skivkontrollen.Standardvärdet är 1. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Hämtar eller anger bredden på varje kolumn i skivkontrollen, i enheten pixlar. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Hämtar eller anger bredden på varje kolumn i skivkontrollen, i enheten pixlar. |
| [GetColumnWidth](./getcolumnwidth/) | Returnerar eller anger bredden på varje kolumn i skivkontrollen i enheten punkter. |
| [SetColumnWidth](./setcolumnwidth/) | Returnerar eller anger bredden på varje kolumn i skivkontrollen i enheten punkter. |
| [GetRowHeightPixel](./getrowheightpixel/) | Returnerar eller anger höjden på varje rad i den angivna skivkontrollen, i enheten pixlar. |
| [SetRowHeightPixel](./setrowheightpixel/) | Returnerar eller anger höjden på varje rad i den angivna skivkontrollen, i enheten pixlar. |
| [GetRowHeight](./getrowheight/) | Returnerar eller anger höjden på varje rad i den angivna skivkontrollen i enheten punkter. |
| [SetRowHeight](./setrowheight/) | Returnerar eller anger höjden på varje rad i den angivna skivkontrollen i enheten punkter. |
