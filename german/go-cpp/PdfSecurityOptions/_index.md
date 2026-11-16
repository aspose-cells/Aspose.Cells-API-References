---
title: "PdfSecurityOptions Klasse"
linktitle: "PdfSecurityOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PdfSecurityOptions Klasse. Kapselt das Objekt, das pdfsecurityoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Optionen zum Verschlüsseln und für Zugriffsberechtigungen eines PDF-Dokuments. PDF/A erlaubt keine Sicherheitseinstellungen.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | Der Konstruktor von PdfSecurityOptions |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetUserPassword](./getuserpassword/) | Liest oder setzt das Benutzerpasswort, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist. |
| [SetUserPassword](./setuserpassword/) | Liest oder setzt das Benutzerpasswort, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist. |
| [GetOwnerPassword](./getownerpassword/) | Liest oder setzt das Besitzerpasswort für das verschlüsselte PDF-Dokument. |
| [SetOwnerPassword](./setownerpassword/) | Liest oder setzt das Besitzerpasswort für das verschlüsselte PDF-Dokument. |
| [GetPrintPermission](./getprintpermission/) | Gibt an, ob das Drucken des Dokuments erlaubt ist. |
| [SetPrintPermission](./setprintpermission/) | Gibt an, ob das Drucken des Dokuments erlaubt ist. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von AnnotationsPermission, FillFormsPermission und AssembleDocumentPermission gesteuerten erlaubt ist. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von AnnotationsPermission, FillFormsPermission und AssembleDocumentPermission gesteuerten erlaubt ist. |
| [GetAnnotationsPermission](./getannotationspermission/) | Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist. |
| [SetAnnotationsPermission](./setannotationspermission/) | Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist. |
| [GetFillFormsPermission](./getfillformspermission/) | Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn ModifyDocumentPermission nicht gesetzt ist. |
| [SetFillFormsPermission](./setfillformspermission/) | Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn ModifyDocumentPermission nicht gesetzt ist. |
| [GetExtractContentPermission](./getextractcontentpermission/) | Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch Vorgänge, die nicht von AccessibilityExtractContent gesteuert werden, erlaubt ist. |
| [SetExtractContentPermission](./setextractcontentpermission/) | Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch Vorgänge, die nicht von AccessibilityExtractContent gesteuert werden, erlaubt ist. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Gibt an, ob das Extrahieren von Text und Grafiken (zur Unterstützung der Barrierefreiheit für Nutzer mit Behinderungen oder zu anderen Zwecken) erlaubt ist. |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Gibt an, ob das Extrahieren von Text und Grafiken (zur Unterstützung der Barrierefreiheit für Nutzer mit Behinderungen oder zu anderen Zwecken) erlaubt ist. |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn ModifyDocumentPermission nicht gesetzt ist. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn ModifyDocumentPermission nicht gesetzt ist. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Gibt an, ob das Drucken des Dokuments zu einer Darstellung, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann, erlaubt ist. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Gibt an, ob das Drucken des Dokuments zu einer Darstellung, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann, erlaubt ist. |
