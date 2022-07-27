---
title: PivotField
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt ein Feld in einem PivotTable-Bericht dar.
type: docs
weight: 4530
url: /de/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Stellt ein Feld in einem PivotTable-Bericht dar.

```csharp
public class PivotField
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Repräsentiert die Anzahl der obersten oder untersten Elemente , die automatisch im angegebenen PivotTable-Feld angezeigt werden. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Repräsentiert den automatisch angezeigten Feldindex. -1 bedeutet PivotField selbst. Es sollte der Index der Datenfelder sein. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Repräsentiert den Feldindex für die automatische Sortierung. -1 bedeutet PivotField selbst, andere bedeutet die Position der Datenfelder. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Stellt das Basisfeld für eine benutzerdefinierte Berechnung dar. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Repräsentiert den PivotField-Index in den Basis-PivotFields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Stellt das Element im Basisfeld für eine benutzerdefinierte Berechnung dar. Gilt nur für Datenfelder. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Stellt das Element im Basisfeld für eine benutzerdefinierte Berechnung dar. Gilt nur für Datenfelder. Da PivotItemPosition.Custom nur zum Lesen dient, müssen Sie, wenn Sie PivotItemPosition.Custom festlegen müssen, das Attribut PivotField.BaseItemIndex festlegen. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Stellt das aktuelle Seitenelement dar, das für das Seitenfeld angezeigt wird (gilt nur für Seitenfelder). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Stellt dar, wie die in einem Datenfeld enthaltenen Werte angezeigt werden. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | Repräsentiert den PivotField-Anzeigenamen. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Gibt an, ob das angegebene Feld an die Spaltenposition gezogen werden kann. Der Standardwert ist wahr. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Gibt an, ob das angegebene Feld an die Datenposition gezogen werden kann. Der Standardwert ist wahr. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Gibt an, ob das angegebene Feld an die Ausblendposition gezogen werden kann. Der Standardwert ist wahr. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Gibt an, ob das angegebene Feld an die Seitenposition gezogen werden kann. Der Standardwert ist wahr. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Gibt an, ob das angegebene Feld an die Zeilenposition gezogen werden kann. Der Standardwert ist wahr. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | Stellt die Funktion dar, die verwendet wird, um das PivotTable-Datenfeld zusammenzufassen. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Gibt an, ob nach jedem Element eine Leerzeile eingefügt wird. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Gibt an, ob das angegebene PivotTable-Feld automatisch aufsteigend angezeigt wird. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Gibt an, ob das angegebene PivotTable-Feld automatisch aufsteigend sortiert ist. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Gibt an, ob das angegebene PivotTable-Feld automatisch angezeigt wird, nur gültig für Excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Gibt an, ob das angegebene PivotTable-Feld automatisch sortiert wird. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist wahr. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Gibt an, ob das angegebene PivotTable-Feld ein berechnetes Feld ist. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | gibt an, ob das Feld neue Elemente im manuellen Filter enthalten kann Der Standardwert ist falsch. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | gibt an, ob das Feld Seitenumbrüche zwischen Artikeln einfügen kann Seitenumbruch nach jedem Artikel einfügen Der Standardwert ist falsch. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | gibt an, ob für das Feld mehrere Elemente auf der Seite ausgewählt werden können field Der Standardwert ist „false“. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | gibt an, ob das Feld Elemente wiederholen kann. labels Der Standardwert ist „false“. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Ruft die Basiselementanzahl dieses Pivot-Felds ab. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Holen Sie sich alle Basisgegenstände; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | Repräsentiert den PivotField-Namen. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Repräsentiert das integrierte Anzeigeformat von Zahlen und Datumsangaben. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Stellt das benutzerdefinierte Anzeigeformat von Zahlen und Datumsangaben dar. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Holen Sie sich die ursprünglichen Basisgegenstände; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Ruft die Pivot-Elemente des Pivot-Felds ab |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | Repräsentiert den PivotField-Index in den PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Ruft den Gruppenbereich des Pivot-Felds ab |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Gibt an, ob alle Elemente im PivotTable-Bericht angezeigt werden, auch wenn sie keine Zusammenfassungsdaten enthalten. Elemente ohne Daten anzeigen Der Standardwert ist „false“. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Gibt an, ob Beschriftungen aus dem nächsten Feld in derselben Spalte in der Pivot-Tabellenansicht angezeigt werden |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Gibt an, ob dieses Feld in Gliederungsform in der Pivot-Tabellenansicht angeordnet ist |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | wenn ShowInOutlineForm wahr ist, dann zeige Zwischensummen oben in der Liste der Elemente statt unten |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Fügen Sie dem Pivot-Feld ein berechnetes Element hinzu. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Abrufen der Formelzeichenfolge des angegebenen berechneten Felds . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | Ruft den Pivot-Filter des Pivot-Felds nach Typ ab |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | Ruft die Pivot-Filter des Pivot-Felds ab |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Ruft ab, ob das angegebene Feld diese Zwischensummen anzeigt. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Legt fest, ob die PivotItems in einem Pivot-Feld ein ausgeblendetes Detail sind. Das heißt, dieses Feld komprimieren/erweitern. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Legt fest, ob das spezifische PivotItem in einem Datenfeld ausgeblendet ist. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Legt fest, ob das spezifische PivotItem in einem Datenfeld ausgeblendet ist. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Legt fest, ob das spezifische PivotItem in einem Pivot-Feld ein ausgeblendetes Detail ist. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Initialisieren Sie die Pivot-Elemente des Pivot-Felds |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Gibt an, ob das spezifische PivotItem ausgeblendet ist. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Gibt an, ob das spezifische PivotItem ein ausgeblendetes Detail ist. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Legt fest, ob das angegebene Feld diese Zwischensummen anzeigt. |

### Beispiele

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

//Attribute von PivotField ändern
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

// Mach dein Geschäft

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

### Siehe auch

* namensraum [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
