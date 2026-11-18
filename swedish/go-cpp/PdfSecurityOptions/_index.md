---
title: "PdfSecurityOptions-klass"
linktitle: "PdfSecurityOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PdfSecurityOptions-klass. Inkapslar objektet som representerar pdfsecurityoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Alternativ för kryptering och åtkomstbehörigheter för ett PDF-dokument. PDF/A tillåter inte säkerhetsinställningar.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | Konstruktorn för PdfSecurityOptions |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetUserPassword](./getuserpassword/) | Hämtar eller anger användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet. |
| [SetUserPassword](./setuserpassword/) | Hämtar eller anger användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet. |
| [GetOwnerPassword](./getownerpassword/) | Hämtar eller anger ägarlösenordet för det krypterade PDF-dokumentet. |
| [SetOwnerPassword](./setownerpassword/) | Hämtar eller anger ägarlösenordet för det krypterade PDF-dokumentet. |
| [GetPrintPermission](./getprintpermission/) | Anger om utskrift av dokumentet ska tillåtas. |
| [SetPrintPermission](./setprintpermission/) | Anger om utskrift av dokumentet ska tillåtas. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | Anger om innehållet i dokumentet får ändras genom operationer som inte styrs av AnnotationsPermission, FillFormsPermission och AssembleDocumentPermission. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | Anger om innehållet i dokumentet får ändras genom operationer som inte styrs av AnnotationsPermission, FillFormsPermission och AssembleDocumentPermission. |
| [GetAnnotationsPermission](./getannotationspermission/) | Anger om textanteckningar får läggas till eller ändras samt om interaktiva formulärfält får fyllas i. |
| [SetAnnotationsPermission](./setannotationspermission/) | Anger om textanteckningar får läggas till eller ändras samt om interaktiva formulärfält får fyllas i. |
| [GetFillFormsPermission](./getfillformspermission/) | Anger om befintliga interaktiva formulärfält (inklusive signaturfält) får fyllas i, även om ModifyDocumentPermission är aktiverad. |
| [SetFillFormsPermission](./setfillformspermission/) | Anger om befintliga interaktiva formulärfält (inklusive signaturfält) får fyllas i, även om ModifyDocumentPermission är aktiverad. |
| [GetExtractContentPermission](./getextractcontentpermission/) | Anger om text och grafik får kopieras eller på annat sätt extraheras från dokumentet genom operationer som inte styrs av AccessibilityExtractContent. |
| [SetExtractContentPermission](./setextractcontentpermission/) | Anger om text och grafik får kopieras eller på annat sätt extraheras från dokumentet genom operationer som inte styrs av AccessibilityExtractContent. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Anger om text och grafik får extraheras (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål). |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Anger om text och grafik får extraheras (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål). |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | Anger om dokumentet får sammanställas (infoga, rotera eller ta bort sidor samt skapa bokmärken eller miniatyrbilder), även om ModifyDocumentPermission är aktiverad. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | Anger om dokumentet får sammanställas (infoga, rotera eller ta bort sidor samt skapa bokmärken eller miniatyrbilder), även om ModifyDocumentPermission är aktiverad. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Anger om dokumentet får skrivas ut till en representation från vilken en exakt digital kopia av PDF-innehållet kan genereras. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Anger om dokumentet får skrivas ut till en representation från vilken en exakt digital kopia av PDF-innehållet kan genereras. |
