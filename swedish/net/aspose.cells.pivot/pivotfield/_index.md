---
title: PivotField
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett fält i en pivottabellrapport.
type: docs
weight: 4530
url: /sv/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Representerar ett fält i en pivottabellrapport.

```csharp
public class PivotField
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Representerar antalet topp- eller bottenobjekt som automatiskt visas i det angivna pivottabellfältet. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Representerar auto show fältindex. -1 betyder själva PivotField. Det bör vara indexet för datafälten. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Representerar fältindex för automatisk sortering. -1 betyder själva PivotField, andra betyder positionen för datafälten. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Representerar basfältet för en anpassad beräkning. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Representerar PivotField-indexet i basen PivotFields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Representerar artikeln i basfältet för en anpassad beräkning. Gäller endast för datafält. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Representerar artikeln i basfältet för en anpassad beräkning. Gäller endast för datafält. Eftersom PivotItemPosition.Custom endast är för läsning, om du behöver ställa in PivotItemPosition.Custom, vänligen ange PivotField.BaseItemIndex attribut. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Representerar det aktuella sidobjektet som visas för sidfältet (gäller endast för sidfält). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Representerar hur man visar värdena som finns i ett datafält. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | Representerar pivotfältets visningsnamn. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Indikerar om det angivna fältet kan dras till kolumnpositionen. Standardvärdet är sant. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Indikerar om det angivna fältet kan dras till datapositionen. Standardvärdet är sant. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Indikerar om det angivna fältet kan dras till gömpositionen. Standardvärdet är sant. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Indikerar om det angivna fältet kan dras till sidpositionen. Standardvärdet är sant. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Indikerar om det angivna fältet kan dras till radpositionen. Standardvärdet är sant. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | Representerar funktionen som används för att sammanfatta pivottabellens datafält. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Anger om tom rad infogas efter varje objekt. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Indikerar om det angivna pivottabellfältet automatiskt visas stigande. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Indikerar om det angivna pivottabellfältet är autosorterat stigande. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Indikerar om det angivna pivottabellfältet visas automatiskt, endast giltigt för excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Indikerar om det angivna pivottabellfältet sorteras automatiskt. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Indikerar om det angivna fältet visar automatiska delsummor. Standard är sant. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Indikerar om det angivna pivottabellfältet är beräknat fält. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | anger om fältet kan inkludera nya objekt i manuellt filter Standardvärdet är falskt. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | anger om fältet kan infoga sidbrytningar mellan items infoga sidbrytningar efter varje item Standardvärdet är falskt. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | anger om fältet kan ha flera items valda på sidan field Standardvärdet är falskt. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | anger om fältet kan upprepa objekt labels Standardvärdet är falskt. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Hämtar basobjektantalet för detta pivotfält. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Få alla basartiklar; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | Representerar pivotfältets namn. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Representerar det inbyggda visningsformatet för siffror och datum. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Representerar det anpassade visningsformatet för siffror och datum. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Skaffa de ursprungliga basartiklarna; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Hämtar pivotposterna för pivotfältet |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | Representerar PivotField-indexet i PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Hämtar gruppintervallet för pivotfältet |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Anger om alla objekt i pivottabellsrapporten visas, även om de inte innehåller sammanfattande data. visa objekt utan data Standardvärdet är falskt. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Indikerar om etiketter från nästa fält i samma kolumn på pivottabellvyn visas |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Anger om layouten av detta fält i konturform på pivottabellen view |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | när ShowInOutlineForm är sant, visa sedan delsummor högst upp i listan över objekt istället för längst ned |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Lägg till ett beräknat objekt i pivotfältet. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Hämta formelsträngen för det angivna beräknade fältet . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | Hämtar pivotfiltret för pivotfältet efter typ |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | Hämtar pivotfiltren för pivotfältet |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Hämtar om det angivna fältet visar dessa delsummor. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Anger om PivotItems i ett pivotfält är dolda detaljer. Det är att komprimera/expandera detta fält. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Anger om den specifika PivotItem i ett datafält är dold. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Anger om den specifika PivotItem i ett datafält är dold. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Anger om den specifika PivotItem i ett pivotfält är dold detalj. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Initiera pivotposterna i pivotfältet |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Indikerar om den specifika PivotItem är dold. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Indikerar om den specifika PivotItem är dold detalj. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Anger om det angivna fältet visar dessa delsummor. |

### Exempel

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Ändra PivotFields attribut
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//gör dina affärer

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Se även

* namnutrymme [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
