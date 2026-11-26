---
title: "Clase PdfSecurityOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions clase. Opciones para encriptar y permisos de acceso de un documento PDF. PDF/A no permite configuraciones de seguridad"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Opciones para el cifrado y los permisos de acceso de un documento PDF. PDF/A no permite configuraciones de seguridad.

```csharp
public class PdfSecurityOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | El constructor de PdfSecurityOptions |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Indica si se permite extraer texto y gráficos (en apoyo de la accesibilidad para usuarios con discapacidades o para otros propósitos). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivos. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o imágenes en miniatura), incluso si [`ModifyDocumentPermission`](./modifydocumentpermission/) está activo. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsoleto.**) Permiso para copiar o extraer contenido Obsoleto según la referencia PDF. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Indica si se permite rellenar campos de formulario interactivos existentes (incluidos los campos de firma), incluso si [`ModifyDocumentPermission`](./modifydocumentpermission/) está activo. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) y [`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Obtiene o establece la contraseña del propietario para el documento PDF encriptado. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Indica si se permite imprimir el documento. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Obtiene o establece la contraseña de usuario requerida para abrir el documento PDF encriptado. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Crear PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Crear PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Establece opciones de seguridad
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

            // Asignar opciones de seguridad a PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Guardar el libro de trabajo como PDF con las opciones de seguridad especificadas
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


