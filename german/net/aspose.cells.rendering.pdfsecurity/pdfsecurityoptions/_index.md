---
title: "Klasse PdfSecurityOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions Klasse. Optionen zum Verschlüsseln und für Zugriffsberechtigungen eines PDF‑Dokuments. PDF/A erlaubt keine Sicherheitseinstellungen."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Optionen zum Verschlüsseln und für Zugriffsberechtigungen eines PDF-Dokuments. PDF/A erlaubt keine Sicherheitseinstellungen.

```csharp
public class PdfSecurityOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | Der Konstruktor von PdfSecurityOptions |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Gibt an, ob das Extrahieren von Text und Grafiken erlaubt ist (zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder zu anderen Zwecken). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn [`ModifyDocumentPermission`](./modifydocumentpermission/) freigegeben ist. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch Operationen, die nicht von [`AccessibilityExtractContent`](./accessibilityextractcontent/) gesteuert werden, erlaubt ist. |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolete.**) Erlaubnis zum Kopieren oder Extrahieren von Inhalten, veraltet gemäß PDF‑Referenz. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn [`ModifyDocumentPermission`](./modifydocumentpermission/) freigegeben ist. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Gibt an, ob das Drucken des Dokuments zu einer Darstellung, aus der eine getreue digitale Kopie des PDF‑Inhalts erzeugt werden kann, erlaubt ist. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Gibt an, ob das Ändern des Inhalts des Dokuments durch Operationen, die nicht von [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) und [`AssembleDocumentPermission`](./assembledocumentpermission/) gesteuert werden, erlaubt ist. |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Liest oder setzt das Besitzerpasswort für das verschlüsselte PDF‑Dokument. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Gibt an, ob das Drucken des Dokuments erlaubt ist. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Liest oder legt das Benutzerkennwort fest, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;

    public class PdfSecurityOptionsDemo
    {
        public static void PdfSecurityOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Erstellen Sie PdfSaveOptions.
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // PdfSecurityOptions erstellen
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Setzen Sie Sicherheitsoptionen
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // Sicherheitsoptionen den PdfSaveOptions zuweisen
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Speichert die Arbeitsmappe als PDF mit den angegebenen Sicherheitsoptionen
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


