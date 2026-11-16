---
title: "PivotField Klasse"
linktitle: "PivotField"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotField Klasse. Kapselt das Objekt, das ein pivotfield in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotfield/
---

## PivotField class

Stellt ein Feld in einem PivotTable-Bericht dar.

```go

type PivotField struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetPivotItems](./getpivotitems/) | Liefert die Pivot-Elemente des Pivot-Feldes |
| [GetMaxValue](./getmaxvalue/) | Liefert den Maximalwert dieses Feldes. |
| [GetMinValue](./getminvalue/) | Liefert den Maximalwert dieses Feldes. |
| [GetGroupSettings](./getgroupsettings/) | Liefert die Gruppeneinstellungen des Pivot-Feldes. |
| [InitPivotItems](./initpivotitems/) | Initialisiert die Pivot-Elemente des Pivot-Feldes |
| [Group](./group/) | Gruppiert das Feld automatisch. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Gruppiert das Pivot-Feld mit Optionen. |
| [GroupBy](./groupby/) | Benutzerdefinierte Gruppierung des Feldes. |
| [Ungroup](./ungroup/) | Gruppierung des Pivot-Feldes aufheben. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Liefert den Pivot-Filter des Pivot-Feldes nach Typ |
| [GetFilters](./getfilters/) | Liefert alle für dieses Pivot-Feld angewendeten Pivot-Filter. |
| [ClearFilter](./clearfilter/) | Löscht die Filtereinstellung dieses Pivot-Feldes. |
| [FilterTop10](./filtertop10/) | Filtert nach Werten des Daten-Pivotfelds. |
| [FilterByValue](./filterbyvalue/) | Filtert nach Werten des Daten-Pivotfelds. |
| [FilterByLabel](./filterbylabel/) | Filtert nach Beschriftungen des Zeilen- oder Spalten-Pivotfelds. |
| [FilterByDate](./filterbydate/) | Filtert nach Datumswerten des Zeilen- oder Spalten-Pivot-Feldes. |
| [IsCalculatedField](./iscalculatedfield/) | Gibt an, ob dieses Pivot-Feld ein berechnetes Feld ist. |
| [GetFormula](./getformula/) | Liefert die Formel des berechneten Feldes. Funktioniert nur für berechnete Felder. |
| [IsValuesField](./isvaluesfield/) | Gibt an, ob dieses Feld ein Wertefeld darstellt. |
| [GetBaseIndex](./getbaseindex/) | Stellt den Index in den Quell-Pivot-Feldern dar. |
| [SetBaseIndex](./setbaseindex/) | Stellt den Index in den Quell-Pivot-Feldern dar. |
| [GetPosition](./getposition/) | Stellt den Index des PivotField in der Region dar. |
| [GetRegionType](./getregiontype/) | Gibt die Region der Pivot‑Tabelle an, in der dieses Feld angezeigt wird. |
| [GetName](./getname/) | Stellt den Namen des PivotField dar. |
| [SetName](./setname/) | Stellt den Namen des PivotField dar. |
| [GetDisplayName](./getdisplayname/) | Stellt den Anzeigenamen des Pivot‑Feldes in der Pivot‑Tabellenansicht dar. |
| [SetDisplayName](./setdisplayname/) | Stellt den Anzeigenamen des Pivot‑Feldes in der Pivot‑Tabellenansicht dar. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Legt fest, wie das angegebene Feld subtotalisiert wird. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Gibt an, ob der angegebene Zwischensumme für dieses Pivot‑Feld angezeigt werden soll. |
| [GetSubtotals](./getsubtotals/) | Liest oder legt die Zwischensummen des Feldes fest. Nur für Zeilen‑ oder Spalten‑Pivot‑Felder. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Liest oder legt die Zwischensummen des Feldes fest. Nur für Zeilen‑ oder Spalten‑Pivot‑Felder. |
| [IsAutoSubtotals](./isautosubtotals/) | Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist wahr. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist wahr. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. Der Standardwert ist wahr. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Gibt an, ob das angegebene Feld in den Zeilenbereich gezogen werden kann. Der Standardwert ist wahr. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist wahr. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Gibt an, ob das angegebene Feld in den Spaltenbereich gezogen werden kann. Der Standardwert ist wahr. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist wahr. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Gibt an, ob das angegebene Feld in den Seitenbereich gezogen werden kann. Der Standardwert ist wahr. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Gibt an, ob dieses Pivot‑Feld aus der PivotTable‑Ansicht entfernt werden kann. Der Standardwert ist wahr. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Gibt an, ob dieses Pivot‑Feld aus der PivotTable‑Ansicht entfernt werden kann. Der Standardwert ist wahr. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. Der Standardwert ist wahr. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Gibt an, ob das angegebene Feld in den Wertebereich gezogen werden kann. Der Standardwert ist wahr. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Gibt an, ob im Seitenfeld mehrere Elemente ausgewählt werden können. Der Standardwert ist falsch. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Gibt an, ob im Seitenfeld mehrere Elemente ausgewählt werden können. Der Standardwert ist falsch. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Gibt an, ob die Beschriftungen des Feldes in der Region wiederholt werden sollen. Der Standardwert ist falsch. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Gibt an, ob die Beschriftungen des Feldes in der Region wiederholt werden sollen. Der Standardwert ist falsch. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Gibt an, ob neue Elemente in das Feld im manuellen Filter aufgenommen werden sollen. Der Standardwert ist falsch. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Gibt an, ob neue Elemente in das Feld im manuellen Filter aufgenommen werden sollen. Der Standardwert ist falsch. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. Der Standardwert ist falsch. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. Der Standardwert ist falsch. |
| [GetShowAllItems](./getshowallitems/) | Gibt an, ob alle Elemente in der PivotTable‑Ansicht angezeigt werden sollen, selbst wenn sie keine Zusammenfassungsdaten enthalten. Der Standardwert ist falsch. |
| [SetShowAllItems](./setshowallitems/) | Gibt an, ob alle Elemente in der PivotTable‑Ansicht angezeigt werden sollen, selbst wenn sie keine Zusammenfassungsdaten enthalten. Der Standardwert ist falsch. |
| [SortBy_SortOrder](./sortby_sortorder/) | Sortiert dieses Pivot‑Feld. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Sortiert dieses Pivot‑Feld. |
| [GetSortSetting](./getsortsetting/) | Liest alle Einstellungen des automatischen Sortierens |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Liest die Top‑10‑AutoShow‑Einstellungen für ein Pivot‑Feld. |
| [Top10AutoShow](./top10autoshow/) | Konfiguriert die Top‑10‑AutoShow‑Einstellungen für dieses Pivot‑Feld. |
| [GetFunction](./getfunction/) | Stellt die Funktion dar, die verwendet wird, um dieses PivotTable‑Datenfeld zusammenzufassen. |
| [SetFunction](./setfunction/) | Stellt die Funktion dar, die verwendet wird, um dieses PivotTable‑Datenfeld zusammenzufassen. |
| [ShowValuesAs](./showvaluesas/) | Zeigt Werte des Datenfeldes in einem anderen Anzeigeformat an, wenn die ShowDataAs‑Berechnung verwendet wird. |
| [GetShowValuesSetting](./getshowvaluessetting/) | Liest die Einstellungen zum Anzeigen von Werten, wenn die ShowDataAs‑Berechnung verwendet wird. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Stellt das aktuell ausgewählte Seitenelement des Seitenfeldes zum Filtern von Daten dar. Nur für Seitenfelder gültig. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Stellt das aktuell ausgewählte Seitenelement des Seitenfeldes zum Filtern von Daten dar. Nur für Seitenfelder gültig. |
| [GetInsertBlankRow](./getinsertblankrow/) | Gibt an, ob nach jedem Element eine leere Zeile eingefügt werden soll. Nur für Zeilenfelder. |
| [SetInsertBlankRow](./setinsertblankrow/) | Gibt an, ob nach jedem Element eine leere Zeile eingefügt werden soll. Nur für Zeilenfelder. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | Gibt an, ob Zwischensummen oben oder unten bei den Elementen angezeigt werden sollen, wenn ShowInOutlineForm true ist, dann |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | Gibt an, ob Zwischensummen oben oder unten bei den Elementen angezeigt werden sollen, wenn ShowInOutlineForm true ist, dann |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Gibt an, ob dieses Feld im Gliederungsformat in der Pivot‑Tabellen‑Ansicht angeordnet werden soll. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Gibt an, ob dieses Feld im Gliederungsformat in der Pivot‑Tabellen‑Ansicht angeordnet werden soll. |
| [GetNumber](./getnumber/) | Stellt das integrierte Anzeigeformat für Zahlen und Datumsangaben dar. |
| [SetNumber](./setnumber/) | Stellt das integrierte Anzeigeformat für Zahlen und Datumsangaben dar. |
| [Get_NumberFormat](./get_numberformat/) | Stellt das benutzerdefinierte Anzeigeformat für Zahlen und Datumsangaben dar. |
| [SetNumberFormat](./setnumberformat/) | Stellt das benutzerdefinierte Anzeigeformat für Zahlen und Datumsangaben dar. |
| [HideAllDetails](./hidealldetails/) | Blendet alle Details aus |
| [ShowAllDetails](./showalldetails/) | Alle Details anzeigen |
| [GetItems](./getitems/) | Alle Beschriftungen der Pivot‑Elemente in diesem Feld abrufen. |
| [GetOriginalItems](./getoriginalitems/) | Die ursprünglichen Basiselemente abrufen; |
| [AddCalculatedItem](./addcalculateditem/) | Ein berechnetes Formelelement zum Pivot‑Feld hinzufügen. |
| [GetShowCompact](./getshowcompact/) | Gibt an, ob die Beschriftungen des nächsten Feldes in derselben Spalte in der Pivot‑Tabellen‑Ansicht angezeigt werden sollen |
| [SetShowCompact](./setshowcompact/) | Gibt an, ob die Beschriftungen des nächsten Feldes in derselben Spalte in der Pivot‑Tabellen‑Ansicht angezeigt werden sollen |
