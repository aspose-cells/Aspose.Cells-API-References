---
title: "ListObject-Klasse"
linktitle: "ListObject"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ListObject-Klasse. Kapselt das Objekt, das listobject in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/listobject/
---

## ListObject class

Stellt eine Tabelle in einem Arbeitsblatt dar.

```go

type ListObject struct  {
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
| [GetStartRow](./getstartrow/) | Gibt die Startzeile des Bereichs zurück. |
| [GetStartColumn](./getstartcolumn/) | Gibt die Startspalte des Bereichs zurück. |
| [GetEndRow](./getendrow/) | Gibt die Endzeile des Bereichs zurück. |
| [GetEndColumn](./getendcolumn/) | Gibt die Endspalte des Bereichs zurück. |
| [GetListColumns](./getlistcolumns/) | Gibt die ListColumn-Liste dieser Tabelle zurück. |
| [Resize](./resize/) | Ändert die Größe des Bereichs des Listobjekts. |
| [PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | Setzt den Wert in die Zelle. |
| [PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | Setzt den Wert in die Zelle. |
| [PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | Setzt die Formel in die Zelle der Tabelle. |
| [PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | Setzt die Formel in die Zelle der Tabelle. |
| [GetShowHeaderRow](./getshowheaderrow/) | Liest und legt fest, ob diese Tabelle die Kopfzeile anzeigt. |
| [SetShowHeaderRow](./setshowheaderrow/) | Liest und legt fest, ob diese Tabelle die Kopfzeile anzeigt. |
| [GetShowTotals](./getshowtotals/) | Liest und legt fest, ob diese TAble die Gesamtsumme-Zeile anzeigt. |
| [SetShowTotals](./setshowtotals/) | Liest und legt fest, ob diese TAble die Gesamtsumme-Zeile anzeigt. |
| [GetDataRange](./getdatarange/) | Gibt den Datenbereich der Tabelle zurück. |
| [UpdateColumnName](./updatecolumnname/) | Aktualisiert die Namen aller ListColumns in den Zellen der Tabelle. |
| [GetQueryTable](./getquerytable/) | Gibt die verknüpfte QueryTable zurück. |
| [GetDataSourceType](./getdatasourcetype/) | Ermittelt den Datentyp der Datenquelle der Tabelle. |
| [GetHasAutoFilter](./gethasautofilter/) | Gibt an, ob ein Auto-Filter auf diese Tabelle angewendet wird. |
| [SetHasAutoFilter](./sethasautofilter/) | Gibt an, ob ein Auto-Filter auf diese Tabelle angewendet wird. |
| [RemoveAutoFilter](./removeautofilter/) | Entfernt den Auto-Filter, der auf diese Tabelle angewendet wurde. |
| [GetAutoFilter](./getautofilter/) | Liest den Auto-Filter dieser Tabelle. |
| [GetDisplayName](./getdisplayname/) | Liest und setzt den Anzeigenamen der Tabelle. |
| [SetDisplayName](./setdisplayname/) | Liest und setzt den Anzeigenamen der Tabelle. |
| [GetComment](./getcomment/) | Liest und setzt den Kommentar der Tabelle. |
| [SetComment](./setcomment/) | Liest und setzt den Kommentar der Tabelle. |
| [GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat. |
| [SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | Gibt an, ob die erste Spalte in der Tabelle den angewendeten Stil hat. |
| [GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat. |
| [SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | Gibt an, ob die letzte Spalte in der Tabelle den angewendeten Stil hat. |
| [GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | Gibt an, ob die Zeilenstreifenformatierung angewendet wird. |
| [SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | Gibt an, ob die Zeilenstreifenformatierung angewendet wird. |
| [GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | Gibt an, ob die Spaltenstreifenformatierung angewendet wird. |
| [SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | Gibt an, ob die Spaltenstreifenformatierung angewendet wird. |
| [ApplyStyleToRange](./applystyletorange/) | Wendet den Tabellestil auf den Bereich an. |
| [ConvertToRange](./converttorange/) | Konvertiert die Tabelle in einen Bereich. |
| [ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | Konvertiert die Tabelle in einen Bereich. |
| [GetTableStyleType](./gettablestyletype/) | Liest den integrierten Tabellestil. |
| [SetTableStyleType](./settablestyletype/) | Liest den integrierten Tabellestil. |
| [GetTableStyleName](./gettablestylename/) | Liest und setzt den Namen des Tabellestils. |
| [SetTableStyleName](./settablestylename/) | Liest und setzt den Namen des Tabellestils. |
| [GetXmlMap](./getxmlmap/) | Liest ein XmlMap, das für diese Liste verwendet wird. |
| [GetAlternativeText](./getalternativetext/) | Liest und setzt den Alternativtext. |
| [SetAlternativeText](./setalternativetext/) | Liest und setzt den Alternativtext. |
| [GetAlternativeDescription](./getalternativedescription/) | Liest und setzt die alternative Beschreibung. |
| [SetAlternativeDescription](./setalternativedescription/) | Liest und setzt die alternative Beschreibung. |
