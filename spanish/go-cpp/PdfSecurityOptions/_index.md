---
title: "Clase PdfSecurityOptions"
linktitle: "PdfSecurityOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase PdfSecurityOptions. Encapsula el objeto que representa pdfsecurityoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Options for encrypting and access permissions for a PDF document.PDF/A does not allow security setting.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | El constructor de PdfSecurityOptions |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetUserPassword](./getuserpassword/) | Obtiene o establece la contraseña de usuario requerida para abrir el documento PDF encriptado. |
| [SetUserPassword](./setuserpassword/) | Obtiene o establece la contraseña de usuario requerida para abrir el documento PDF encriptado. |
| [GetOwnerPassword](./getownerpassword/) | Obtiene o establece la contraseña del propietario para el documento PDF encriptado. |
| [SetOwnerPassword](./setownerpassword/) | Obtiene o establece la contraseña del propietario para el documento PDF encriptado. |
| [GetPrintPermission](./getprintpermission/) | Indica si se permite imprimir el documento. |
| [SetPrintPermission](./setprintpermission/) | Indica si se permite imprimir el documento. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por AnnotationsPermission, FillFormsPermission y AssembleDocumentPermission. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por AnnotationsPermission, FillFormsPermission y AssembleDocumentPermission. |
| [GetAnnotationsPermission](./getannotationspermission/) | Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivos. |
| [SetAnnotationsPermission](./setannotationspermission/) | Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivos. |
| [GetFillFormsPermission](./getfillformspermission/) | Indica si se permite rellenar campos de formulario interactivos existentes (incluidos los campos de firma), incluso si ModifyDocumentPermission está habilitado. |
| [SetFillFormsPermission](./setfillformspermission/) | Indica si se permite rellenar campos de formulario interactivos existentes (incluidos los campos de firma), incluso si ModifyDocumentPermission está habilitado. |
| [GetExtractContentPermission](./getextractcontentpermission/) | Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por AccessibilityExtractContent. |
| [SetExtractContentPermission](./setextractcontentpermission/) | Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por AccessibilityExtractContent. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Indica si se permite extraer texto y gráficos (para apoyar la accesibilidad a usuarios con discapacidades o para otros propósitos). |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Indica si se permite extraer texto y gráficos (para apoyar la accesibilidad a usuarios con discapacidades o para otros propósitos). |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o miniaturas), incluso si ModifyDocumentPermission está habilitado. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o miniaturas), incluso si ModifyDocumentPermission está habilitado. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF. |
