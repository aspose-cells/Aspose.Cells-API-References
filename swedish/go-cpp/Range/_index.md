---
title: "Range-klass"
linktitle: "Range"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Range-klass. Inkapslar objektet som representerar range i Go."
type: docs
weight: 200
url: /sv/go-cpp/range/
---

## Range class

Inkapslar objektet som representerar ett område av celler i ett kalkylblad.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | Klasskonstruktor. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | Klasskonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [AutoFill_Range](./autofill_range/) | Fyll automatiskt målintervallet. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Fyll automatiskt målintervallet. |
| [GetCurrentRegion](./getcurrentregion/) | Returnerar ett Range-objekt som representerar den aktuella regionen. Den aktuella regionen är ett intervall som begränsas av någon kombination av tomma rader och tomma kolumner. |
| [GetHyperlinks](./gethyperlinks/) | Hämtar alla hyperlänkar i intervallet. |
| [AddHyperlink](./addhyperlink/) | Lägger till en hyperlänk till en specificerad cell eller ett cellintervall. |
| [GetEnumerator](./getenumerator/) | Hämtar enumeratorn för celler i detta Range. |
| [IsIntersect](./isintersect/) | Indikerar om intervallet skär varandra. |
| [Intersect](./intersect/) | Returnerar ett Range-objekt som representerar den rektangulära skärningen av två intervall. |
| [UnionRanges](./unionranges/) | Returnerar unionsresultatet av två intervall. |
| [GetRowCount](./getrowcount/) | Hämtar antalet rader i intervallet. |
| [GetColumnCount](./getcolumncount/) | Hämtar antalet kolumner i intervallet. |
| [GetName](./getname/) | Hämtar eller anger namnet på området. |
| [SetName](./setname/) | Hämtar eller anger namnet på området. |
| [GetRefersTo](./getrefersto/) | Hämtar vad området refererar till. |
| [GetAddress](./getaddress/) | Hämtar adressen för området. |
| [IsBlank](./isblank/) | Anger om området innehåller värden. |
| [GetLeft](./getleft/) | Hämtar avståndet, i punkter, från den vänstra kanten av kolumn A till den vänstra kanten av området. |
| [GetTop](./gettop/) | Hämtar avståndet, i punkter, från den övre kanten av rad 1 till den övre kanten av området. |
| [GetWidth](./getwidth/) | Hämtar bredden på ett område i punkter. |
| [GetHeight](./getheight/) | Hämtar bredden på ett område i punkter. |
| [GetFirstRow](./getfirstrow/) | Hämtar indexet för den första raden i området. |
| [GetFirstColumn](./getfirstcolumn/) | Hämtar indexet för den första kolumnen i området. |
| [Merge](./merge/) | Kombinerar ett cellområde till en enda cell. |
| [UnMerge](./unmerge/) | Delar upp sammanslagna celler i detta område. |
| [PutValue](./putvalue/) | Sätter ett värde i området, om lämpligt kommer värdet att konverteras till en annan datatyp och cellens talformat återställas. |
| [GetValue](./getvalue/) | Hämtar och anger värdet för området. |
| [SetValue](./setvalue/) | Hämtar och anger värdet för området. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Applicera cellstilen. |
| [ApplyStyle](./applystyle/) | Tillämpar format för ett helt område. |
| [SetStyle_Style](./setstyle_style/) | Anger stilen för området. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Anger konturkanterna runt ett cellområde med samma kantstil och färg. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Anger konturkanterna runt ett cellområde med samma kantstil och färg. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Anger konturkanter runt ett cellområde. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Anger konturkant runt ett cellområde. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Anger konturkant runt ett cellområde. |
| [SetInsideBorders](./setinsideborders/) | Ange inre kanter för området. |
| [GetColumnWidth](./getcolumnwidth/) | Anger eller hämtar kolumnbredden för detta område. |
| [SetColumnWidth](./setcolumnwidth/) | Anger eller hämtar kolumnbredden för detta område. |
| [GetRowHeight](./getrowheight/) | Anger eller hämtar höjden på raderna i detta område. |
| [SetRowHeight](./setrowheight/) | Anger eller hämtar höjden på raderna i detta område. |
| [MoveTo](./moveto/) | Flytta det aktuella området till destinationsområdet. |
| [CopyData](./copydata/) | Kopierar celldata (inklusive formler) från ett källområde. |
| [CopyValue](./copyvalue/) | Kopierar cellvärde från ett källområde. |
| [CopyStyle](./copystyle/) | Kopierar stilinställningar från ett källintervall. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Kopierar intervallet med specialklistra in-alternativ. |
| [Transpose](./transpose/) | Transponera (rotera) data från rader till kolumner eller omvänt. |
| [Copy_Range](./copy_range/) | Kopierar data (inklusive formler), formatering, ritobjekt etc. från ett källintervall. |
| [Get](./get/) | Hämtar Cell-objekt i detta intervall. |
| [GetCellOrNull](./getcellornull/) | Hämtar Cell-objekt eller null i detta intervall. |
| [GetOffset](./getoffset/) | Hämtar Range-intervall med förskjutning. |
| [GetEntireColumn](./getentirecolumn/) | Hämtar ett Range-objekt som representerar hela kolumnen (eller kolumnerna) som innehåller det angivna intervallet. |
| [GetEntireRow](./getentirerow/) | Hämtar ett Range-objekt som representerar hela raden (eller raderna) som innehåller det angivna intervallet. |
| [GetWorksheet](./getworksheet/) | Hämtar Worksheet-objektet som innehåller detta intervall. |
| [ToString](./tostring/) | Returnerar en sträng som representerar det aktuella Range-objektet. |
| [ToImage](./toimage/) | Konverterar intervallet till bild. |
| [ToJson](./tojson/) | Konvertera intervallet till JSON-värde. |
| [ToHtml](./tohtml/) | Konvertera intervallet till HTML. |
| [Clear](./clear/) | Rensar detta intervall. |
| [ClearContents](./clearcontents/) | Rensar innehållet i detta intervall. |
| [ClearFormats](./clearformats/) | Rensar formaten för detta intervall. |
| [ClearComments](./clearcomments/) | Rensar kommentarerna i detta intervall. |
| [ClearHyperlinks](./clearhyperlinks/) | Tar bara bort hyperlänkar. |
