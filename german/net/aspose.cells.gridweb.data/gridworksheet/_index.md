---
title: "Klasse GridWorksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet class. Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Kapselt das Objekt, das ein einzelnes Arbeitsblatt darstellt.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Liest oder setzt die aktive Zelle im Arbeitsblatt. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Liest und setzt das Hintergrundbild des Arbeitsblatts. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Binden Sie die Spaltensammlung. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | Das tatsächlich zur Laufzeit bindende Datenquellenobjekt. Es ist ein DataView-Objekt, wenn die DataSource-Eigenschaft ein DataSet-, DataTable- oder DataView-Objekt ist. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die Datenquelle gebunden werden soll. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die Datenquelle gebunden werden soll. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Liefert die [`GridCell`](../gridcell/) Sammlung. |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Stellt den Code-Namen des Arbeitsblatts dar. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Liefert die [`GridComment`](../gridcomment/) Sammlung. |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Liefert die Anzahl der Bindungszeilen im Datenbindungsmodus. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Liest oder setzt das DataMember der mehrgliedrigen DataSource. Im Allgemeinen stellt es ein DataTable-Objekt eines DataSet dar. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Liest oder setzt die DataSource. Im Allgemeinen ist es ein DataSet-Objekt. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Gibt an, ob das angegebene Arbeitsblatt von rechts nach links statt von links nach rechts angezeigt wird. Standard ist false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | Wahr, wenn Nullwerte angezeigt werden. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | Im Datenbindungsmodus gibt an, ob Spaltenkopfbeschriftungen im Blatt erstellt werden sollen. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Stellt den Index der ersten sichtbaren Spalte dar. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Stellt den Index der ersten sichtbaren Zeile dar. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Liest oder setzt die aktive Zelle im Arbeitsblatt. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Liefert die [`GridHyperlinkCollection`](../gridhyperlinkcollection/) Sammlung. |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Ruft den Index des Blatts in der Arbeitsblatt-Sammlung ab. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Rasterlinien sichtbar sind. Standard ist true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Liest oder setzt den Namen des Arbeitsblatts. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Gibt an, ob die Gliederung angezeigt wird. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Liefert eine [`Pictures`](./pictures/) Sammlung. |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Liefert die PivotTables im Arbeitsblatt. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Gibt an, ob dieses Arbeitsblatt beim Öffnen der Arbeitsmappe ausgewählt ist. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Liefert eine [`Pictures`](./pictures/) Sammlung. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixeln. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Stellt die Registerkartenfarbe des Arbeitsblatts dar. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten der Steuerung angezeigt wird. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Liefert das [`GridWorkbook`](../gridworkbook/) Objekt der Arbeitsblatt-Sammlung. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Stellt den Skalierungsfaktor in Prozent dar. Er sollte zwischen 10 und 400 liegen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Fügt einen benutzerdefinierten Filter für die angegebene Zeile hinzu. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Passt die Spaltenbreite automatisch an. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Passt die Zeilenhöhe automatisch an. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Passt die Zeilenhöhe automatisch an. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Passt die Zeilenhöhe in einem rechteckigen Bereich automatisch an. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Passt alle Zeilen in diesem Arbeitsblatt automatisch an. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Passt die Zeilenhöhe in einem Bereich automatisch an. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Berechnet eine Formel. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Bricht ab und löscht die neu hinzugefügte Bindungszeile. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Löscht alle Kommentare im Designer-Tabellenblatt. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Bestätigt die neu hinzugefügte Bindungszeile und fügt sie der Datenquelle hinzu. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Kopiert Inhalte und Formate von einem anderen Arbeitsblatt. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | Nachdem eine Datenquelle für das Arbeitsblatt festgelegt wurde, rufen Sie diese Methode auf, um die Bindungsspalten automatisch zu erzeugen. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Erstellt eine neue Bindungszeile und bindet sie an die Datenquelle. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Erstellt eine Zwischensumme im Blatt. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Erstellt eine Zwischensumme im Blatt. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Bindet das Blatt an die DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Bindet das Blatt an die DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Löscht eine Bindungszeile. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Setzt den Filter für die Spalte. Hinweis: Wir sollten AddAutoFilter aufrufen, bevor filterString verwendet wird. Der Filterkriterien-String. Hinweis: Wir verwenden das Komma-&gt;"," als Trennzeichen, daher darf der zu filternde Zellenwert kein Komma enthalten. filterString(10,"123,456") bedeutet, dass Spalte 10 123 oder 456 enthält, filterString(10,"123") bedeutet, dass Spalte 10 123 enthält, der Spaltenindexwert wird durch Komma getrennt, z.B. 123,456,789 oder abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Liefert die Spaltenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird ein leerer String zurückgegeben. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Liefert den Tooltip-Text der Spaltenüberschrift. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Ermittelt, ob eine Spalte schreibgeschützt ist. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Liest die eingefrorenen Bildschirmelemente. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Ermittelt, ob die Zelle schreibgeschützt ist. Dies ist ein erweitertes Attribut von GridWeb, es wird in der tatsächlichen Excel-Datei nicht beibehalten. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Liefert die Zeilenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird eine leere Zeichenkette zurückgegeben. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Liefert den Tooltip-Text der Zeilenüberschrift. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Ermittelt, ob eine Zeile schreibgeschützt ist. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Gruppiert Zeilen. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Gibt an, ob das Arbeitsblatt geschützt ist. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Verschiebt das Blatt an einen anderen Ort im Tabellenblatt. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Aktualisiere AutoFilter, um Zeilen auszublenden oder wieder einzublenden. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Entfernt den Auto-Filter des Arbeitsblatts. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Entfernt die Zwischensumme, die durch die Methode CreateSubtotal im Blatt erstellt wurde. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | Der ganzzahlige Versatz des Feldes, auf das Sie anwenden möchten, basierend auf der ersten Filterspalte (von links in der Liste; das linkeste Feld ist Feld 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Macht alle Zellen editierbar. Dies ist ein erweitertes Attribut. |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Macht alle Zellen schreibgeschützt. Dies ist ein erweitertes Attribut; beachten Sie, dass dieses Attribut in der tatsächlichen Zelle nicht beibehalten wird. Wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Setzt die Beschriftung für die Spalte. Bitte beachten Sie, dass dies ein erweitertes Attribut ist und nicht in der Excel-Datei beibehalten werden kann. |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Setzt den Tooltip-Text der Spaltenüberschrift. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Setzt eine Spalte auf schreibgeschützt, sodass der Benutzer sie nicht von der Clientseite löschen kann. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Macht alle Zellen schreibgeschützt, indem die Methode SetAllCellsReadonly aufgerufen wird. Rufen Sie anschließend diese Methode auf, um den Zellbereich festzulegen, der editierbar sein soll. |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Legt fest, ob die Zelle schreibgeschützt ist. Dies ist ein erweitertes Attribut von GridWeb, es wird in der tatsächlichen Excel-Datei nicht beibehalten. |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Schützt das Arbeitsblatt. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem die Methode SetAllCellsEditable aufgerufen wird. Dann diese Methode aufrufen, um den Zellbereich festzulegen, der schreibgeschützt sein soll. |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Setzt die Beschriftung für die Zeile. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Setzt den Tooltip-Text der Zeilenüberschrift. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Setzt eine Zeile auf schreibgeschützt, sodass der Benutzer sie nicht von der Clientseite löschen kann. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Löst das Einfrieren von Bereichen im Arbeitsblatt auf. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Löst die Gruppierung von Zeilen auf. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Entfernt den Schutz des Arbeitsblatts. |

## Ereignisse

| Name | Beschreibung |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Tritt auf, wenn das Arbeitsblatt eine neue Bindungszeile erstellt hat und diese initialisiert werden muss. |

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


