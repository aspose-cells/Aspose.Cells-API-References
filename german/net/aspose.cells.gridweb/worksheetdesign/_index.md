---
title: "Klasse WorksheetDesign"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.WorksheetDesign Klasse. Erbt von WebWorksheet. Wird nur zur Entwurfszeit verwendet."
type: docs
url: /de/net/aspose.cells.gridweb/worksheetdesign/
---
## WorksheetDesign class

Erbt von WebWorksheet. Nur zur Designzeit verwendet.

```csharp
public class WorksheetDesign : WebWorksheet
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WorksheetDesign](worksheetdesign/#constructor)() | Standardkonstruktor. |
| [WorksheetDesign](worksheetdesign/#constructor_1)(MainWeb, GridWorksheet) | Der Konstruktor mit MainWeb und GridWorksheet |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Bind-Spalten-Sammlung.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | Das tatsächlich zur Laufzeit bindende Datenquellenobjekt. Es ist ein DataView-Objekt, wenn die DataSource-Eigenschaft ein DataSet-, DataTable- oder DataView-Objekt ist.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die Datenquelle gebunden wird.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die Datenquelle gebunden wird.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } | (Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Ruft die [`WebCells`](../../aspose.cells.gridweb.data/webcells/) ab.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } | (Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Ruft die Anzahl der Bindungszeilen im Datenbindungsmodus ab.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Liest oder setzt das DataMember aus der mehrgliedrigen DataSource. Im Allgemeinen stellt es ein DataTable-Objekt eines DataSet dar.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Liest oder setzt die DataSource. Im Allgemeinen ist es ein DataSet-Objekt.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | Im Datenbindungsmodus gibt an, ob Spaltenkopfzeilenbeschriftungen im Blatt erstellt werden sollen.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Ruft die HyperlinkCollection-Sammlung ab.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Ruft den Index von sich selbst innerhalb der Arbeitsblätter ab.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Liest oder setzt, ob das Arbeitsblatt geschützt ist. Wenn ein Arbeitsblatt geschützt ist, können alle Zellen nicht bearbeitet werden, außer der Zelle, deren IsLocked-Eigenschaft false ist.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Liest oder setzt den Namen des Blatts.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } | (Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Ruft die Datengültigkeits-Einstellungs-Sammlung im Arbeitsblatt ab.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten der Steuerung angezeigt wird.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int) | Passt die Spaltenbreite automatisch an.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int, int, int) | Passt die Spaltenbreite automatisch an. Diese Methode passt eine Spalte basierend auf dem Inhalt eines Zellbereichs innerhalb der Spalte von startRow bis endRow an. AutoFitColumn ist eine ungenaue Funktion.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Bricht die neu hinzugefügte Bindungszeile ab und löscht sie.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Bestätigt die neu hinzugefügte Bindungszeile und fügt sie der Datenquelle hinzu.(Inherited from [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Kopien von einem anderen Arbeitsblattobjekt.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Nachdem ein Datenquelle für das Arbeitsblatt festgelegt wurde, rufen Sie diese Methode auf, um die Bindespalten automatisch zu erzeugen.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Erstellt eine neue Bindereihe und bindet sie an die Datenquelle.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Erstellt eine Zwischensumme im Blatt.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Binden Sie das Blatt an die Datenquelle.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Löscht eine Bindereihe.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Friert die Bereiche an der angegebenen Zelle im Arbeitsblatt ein.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int) | Gruppiert Zeilen.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int, bool) | Gruppiert Zeilen.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Macht alle Zellen editierbar.dies ist ein erweitertes Attribut(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Macht alle Zellen schreibgeschützt.dies ist ein erweitertes Attribut Hinweis, dass dieses Attribut nicht in der tatsächlichen Zelle erhalten werden kann; wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Macht alle Zellen schreibgeschützt, indem Sie die Methode SetAllCellsReadonly aufrufen. Rufen Sie dann diese Methode auf, um den Zellbereich festzulegen, der editierbar sein soll(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem Sie die Methode SetAllCellsEditable aufrufen. Rufen Sie dann diese Methode auf, um den Zellbereich festzulegen, der schreibgeschützt sein soll(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Löst das Einfrieren von Bereichen im Arbeitsblatt auf.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Löst die Gruppierung von Zeilen auf.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Aktualisiert den Eigenschaftswert des Bindungs-Datenquellendatensatzes gemäß dem Zellenwert.(Geerbt von [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

### Siehe auch

* class [WebWorksheet](../../aspose.cells.gridweb.data/webworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


