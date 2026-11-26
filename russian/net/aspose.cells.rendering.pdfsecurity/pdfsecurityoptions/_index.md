---
title: "Класс PdfSecurityOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions. Параметры шифрования и прав доступа для PDF‑документа. PDF/A не допускает настройки безопасности."
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Параметры шифрования и прав доступа для PDF‑документа. PDF/A не допускает настройки безопасности.

```csharp
public class PdfSecurityOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | Конструктор класса PdfSecurityOptions |

## Свойства

| Имя | Описание |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Указывает, разрешено ли извлекать текст и графику (в целях обеспечения доступности для пользователей с ограниченными возможностями или для других целей). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля формы. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если [`ModifyDocumentPermission`](./modifydocumentpermission/) разрешён. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Указывает, разрешено ли копировать или иным способом извлекать текст и графику из документа операциями, отличными от контролируемых [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolete.**) Разрешение копировать или извлекать содержимое устарело согласно справочнику PDF. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Указывает, разрешено ли заполнять существующие интерактивные поля формы (включая поля подписи), даже если [`ModifyDocumentPermission`](./modifydocumentpermission/) разрешён. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Указывает, разрешено ли печатать документ в виде, из которого можно создать точную цифровую копию содержимого PDF. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) и [`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Получает или задаёт пароль владельца зашифрованного PDF‑документа. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Указывает, разрешено ли печатать документ. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Получает или задаёт пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Создать PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Создать PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Установите параметры безопасности
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

            // Назначить параметры безопасности для PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Сохранить книгу в формате PDF с указанными параметрами безопасности
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


