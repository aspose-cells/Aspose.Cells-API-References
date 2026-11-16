---
title: "Style-Klasse"
linktitle: "Style"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Style-Klasse. Kapselt das Objekt, das Style in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/style/
---

## Style class

Stellt den Anzeigestil eines Excel-Dokuments dar, wie Schriftart, Farbe, Ausrichtung, Rahmen usw. Das Style‑Objekt enthält alle Stilattribute (Schriftart, Zahlenformat, Ausrichtung usw.) als Eigenschaften.

```go

type Style struct  {
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
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | Liefert und legt die Hintergrund-Designfarbe fest. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | Liefert und legt die Hintergrund-Designfarbe fest. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | Liefert und legt die Vordergrund-Designfarbe fest. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | Liefert und legt die Vordergrund-Designfarbe fest. |
| [GetName](./getname/) | Liefert oder legt den Namen des Stils fest. |
| [SetName](./setname/) | Liefert oder legt den Namen des Stils fest. |
| [GetPattern](./getpattern/) | Liefert oder legt den Zellhintergrund-Mustertyp fest. |
| [SetPattern](./setpattern/) | Liefert oder legt den Zellhintergrund-Mustertyp fest. |
| [SetPatternColor](./setpatterncolor/) | Legt die Hintergrundfarbe fest. |
| [GetBorders](./getborders/) | Liefert die BorderCollection des Stils. |
| [GetBackgroundColor](./getbackgroundcolor/) | Liefert oder legt die Hintergrundfarbe eines Stils fest. |
| [SetBackgroundColor](./setbackgroundcolor/) | Liefert oder legt die Hintergrundfarbe eines Stils fest. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | Liefert und legt die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert fest. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | Liefert und legt die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert fest. |
| [GetForegroundColor](./getforegroundcolor/) | Liefert oder legt die Vordergrundfarbe eines Stils fest. |
| [SetForegroundColor](./setforegroundcolor/) | Liefert oder legt die Vordergrundfarbe eines Stils fest. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | Liest und setzt die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | Liest und setzt die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert. |
| [Copy](./copy/) | Kopiert Daten von einem anderen Stilobjekt |
| [GetHasBorders](./gethasborders/) | Prüft, ob für den Stil Rahmen gesetzt wurden. |
| [GetParentStyle](./getparentstyle/) | Liest den übergeordneten Stil dieses Stils. |
| [Update](./update/) | Wendet den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. Es funktioniert wie das Klicken auf die Schaltfläche "OK", nachdem Sie den Stil bearbeitet haben. Gilt nur für benannte Stile. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | Gibt an, ob die Zahlenformatierung angewendet werden soll. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | Gibt an, ob die Zahlenformatierung angewendet werden soll. |
| [IsFontApplied](./isfontapplied/) | Gibt an, ob die Schriftformatierung angewendet werden soll. |
| [SetIsFontApplied](./setisfontapplied/) | Gibt an, ob die Schriftformatierung angewendet werden soll. |
| [IsAlignmentApplied](./isalignmentapplied/) | Gibt an, ob die Ausrichtungsformatierung angewendet werden soll. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | Gibt an, ob die Ausrichtungsformatierung angewendet werden soll. |
| [IsBorderApplied](./isborderapplied/) | Gibt an, ob die Rahmenformatierung angewendet werden soll. |
| [SetIsBorderApplied](./setisborderapplied/) | Gibt an, ob die Rahmenformatierung angewendet werden soll. |
| [IsFillApplied](./isfillapplied/) | Gibt an, ob die Füllformatierung angewendet werden soll. |
| [SetIsFillApplied](./setisfillapplied/) | Gibt an, ob die Füllformatierung angewendet werden soll. |
| [IsProtectionApplied](./isprotectionapplied/) | Gibt an, ob die Schutzformatierung angewendet werden soll. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | Gibt an, ob die Schutzformatierung angewendet werden soll. |
| [IsModified](./ismodified/) | Prüft, ob die angegebenen Eigenschaften des Stils geändert wurden. Wird für den Stil von ConditionalFormattings verwendet, um zu prüfen, ob die angegebenen Eigenschaften dieses Stils beim Anwenden von ConditionalFormattings auf eine Zelle verwendet werden sollen. |
| [Equals](./equals/) | Bestimmt, ob zwei Style‑Instanzen gleich sind. |
| [GetHashCode](./gethashcode/) | Dient als Hash‑Funktion für ein Style‑Objekt. |
| [GetIndentLevel](./getindentlevel/) | Stellt die Einrückungsebene für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 250 sein. |
| [SetIndentLevel](./setindentlevel/) | Stellt die Einrückungsebene für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 250 sein. |
| [GetFont](./getfont/) | Liest ein Font‑Objekt. |
| [GetRotationAngle](./getrotationangle/) | Stellt den Textrotationswinkel dar. |
| [SetRotationAngle](./setrotationangle/) | Stellt den Textrotationswinkel dar. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | Liest oder setzt den horizontalen Ausrichtungstyp des Textes in einer Zelle. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | Liest oder setzt den horizontalen Ausrichtungstyp des Textes in einer Zelle. |
| [GetVerticalAlignment](./getverticalalignment/) | Liest oder setzt den vertikalen Ausrichtungstyp des Textes in einer Zelle. |
| [SetVerticalAlignment](./setverticalalignment/) | Liest oder setzt den vertikalen Ausrichtungstyp des Textes in einer Zelle. |
| [IsTextWrapped](./istextwrapped/) | Liest oder setzt einen Wert, der angibt, ob der Text in einer Zelle umgebrochen wird. |
| [SetIsTextWrapped](./setistextwrapped/) | Liest oder setzt einen Wert, der angibt, ob der Text in einer Zelle umgebrochen wird. |
| [GetNumber](./getnumber/) | Liest oder setzt das Anzeigeformat von Zahlen und Datumsangaben. Die Formatierungsmuster unterscheiden sich je nach Region. |
| [SetNumber](./setnumber/) | Liest oder setzt das Anzeigeformat von Zahlen und Datumsangaben. Die Formatierungsmuster unterscheiden sich je nach Region. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Setzt die Rahmen des Stils. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Setzt die Rahmen des Stils. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Setzt die Konturrahmen |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Setzt die Konturrahmen |
| [IsLocked](./islocked/) | Liest oder setzt einen Wert, der angibt, ob eine Zelle bearbeitet werden kann oder nicht. |
| [SetIsLocked](./setislocked/) | Liest oder setzt einen Wert, der angibt, ob eine Zelle bearbeitet werden kann oder nicht. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | Setzt die benutzerdefinierte Zahlenformatzeichenfolge einer Zelle. |
| [GetCustom](./getcustom/) | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Stilobjekts dar. Wenn das benutzerdefinierte Zahlenformat nicht festgelegt ist (Zum Beispiel ist das Zahlenformat eingebaut), "" wird zurückgegeben. |
| [SetCustom_String](./setcustom_string/) | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Stilobjekts dar. Wenn das benutzerdefinierte Zahlenformat nicht festgelegt ist (Zum Beispiel ist das Zahlenformat eingebaut), "" wird zurückgegeben. |
| [GetCultureCustom](./getculturecustom/) | Liest und setzt die kulturbasierte Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben. |
| [SetCultureCustom](./setculturecustom/) | Liest und setzt die kulturbasierte Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben. |
| [GetInvariantCustom](./getinvariantcustom/) | Liest die kulturunabhängige Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben. |
| [IsFormulaHidden](./isformulahidden/) | Gibt an, ob die Formel ausgeblendet wird, wenn das Arbeitsblatt geschützt ist. |
| [SetIsFormulaHidden](./setisformulahidden/) | Gibt an, ob die Formel ausgeblendet wird, wenn das Arbeitsblatt geschützt ist. |
| [GetShrinkToFit](./getshrinktofit/) | Gibt an, ob Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [SetShrinkToFit](./setshrinktofit/) | Gibt an, ob Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [GetTextDirection](./gettextdirection/) | Stellt die Lesereihenfolge des Textes dar. |
| [SetTextDirection](./settextdirection/) | Stellt die Lesereihenfolge des Textes dar. |
| [IsJustifyDistributed](./isjustifydistributed/) | Gibt an, ob für die letzte Textzeile die Block- oder verteilte Ausrichtung der Zellen verwendet werden soll. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | Gibt an, ob für die letzte Textzeile die Block- oder verteilte Ausrichtung der Zellen verwendet werden soll. |
| [GetQuotePrefix](./getquoteprefix/) | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [SetQuotePrefix](./setquoteprefix/) | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [IsGradient](./isgradient/) | Gibt an, ob die Zellenfüllung ein Farbverlaufsmuster ist. |
| [SetIsGradient](./setisgradient/) | Gibt an, ob die Zellenfüllung ein Farbverlaufsmuster ist. |
| [SetTwoColorGradient](./settwocolorgradient/) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | Liest die Einstellung des Zweifarbverlaufs. |
| [IsPercent](./ispercent/) | Gibt an, ob das Zahlenformat ein Prozentformat ist. |
| [IsDateTime](./isdatetime/) | Gibt an, ob das Zahlenformat ein Datumsformat ist. |
| [IsCheckBox](./ischeckbox/) | Gibt an, ob es sich um einen Stil einer Checkbox handelt |
| [SetIsCheckBox](./setischeckbox/) | Gibt an, ob es sich um einen Stil einer Checkbox handelt |
| [ToJson](./tojson/) | Konvertiert Stil in JSON-Strukturdaten. |
| [GetLeftBorder](./getleftborder/) | Liest den linken Rand. |
| [GetRightBorder](./getrightborder/) | Liest den rechten Rand. |
| [GetTopBorder](./gettopborder/) | Liest den oberen Rand. |
| [GetBottomBorder](./getbottomborder/) | Liest den unteren Rand. |
