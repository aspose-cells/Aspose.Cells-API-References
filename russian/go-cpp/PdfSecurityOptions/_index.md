---
title: "Класс PdfSecurityOptions"
linktitle: "PdfSecurityOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PdfSecurityOptions. Инкапсулирует объект, представляющий pdfsecurityoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Параметры шифрования и прав доступа для PDF‑документа. PDF/A не допускает настройки безопасности.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | Конструктор PdfSecurityOptions |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetUserPassword](./getuserpassword/) | Получает или устанавливает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа. |
| [SetUserPassword](./setuserpassword/) | Получает или устанавливает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа. |
| [GetOwnerPassword](./getownerpassword/) | Получает или устанавливает пароль владельца для зашифрованного PDF‑документа. |
| [SetOwnerPassword](./setownerpassword/) | Получает или устанавливает пароль владельца для зашифрованного PDF‑документа. |
| [GetPrintPermission](./getprintpermission/) | Указывает, разрешено ли печатать документ. |
| [SetPrintPermission](./setprintpermission/) | Указывает, разрешено ли печатать документ. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых AnnotationsPermission, FillFormsPermission и AssembleDocumentPermission. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых AnnotationsPermission, FillFormsPermission и AssembleDocumentPermission. |
| [GetAnnotationsPermission](./getannotationspermission/) | Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля формы. |
| [SetAnnotationsPermission](./setannotationspermission/) | Указывает, разрешено ли добавлять или изменять текстовые аннотации, заполнять интерактивные поля формы. |
| [GetFillFormsPermission](./getfillformspermission/) | Указывает, разрешено ли заполнять существующие интерактивные поля формы (включая поля подписи), даже если ModifyDocumentPermission снят. |
| [SetFillFormsPermission](./setfillformspermission/) | Указывает, разрешено ли заполнять существующие интерактивные поля формы (включая поля подписи), даже если ModifyDocumentPermission снят. |
| [GetExtractContentPermission](./getextractcontentpermission/) | Указывает, разрешено ли копировать или иным образом извлекать текст и графику из документа операциями, отличными от контролируемых AccessibilityExtractContent. |
| [SetExtractContentPermission](./setextractcontentpermission/) | Указывает, разрешено ли копировать или иным образом извлекать текст и графику из документа операциями, отличными от контролируемых AccessibilityExtractContent. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Указывает, разрешено ли извлекать текст и графику (в целях обеспечения доступности для пользователей с ограниченными возможностями или для других целей). |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Указывает, разрешено ли извлекать текст и графику (в целях обеспечения доступности для пользователей с ограниченными возможностями или для других целей). |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если ModifyDocumentPermission снят. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если ModifyDocumentPermission снят. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Указывает, разрешено ли печатать документ в представление, из которого можно создать точную цифровую копию содержимого PDF. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Указывает, разрешено ли печатать документ в представление, из которого можно создать точную цифровую копию содержимого PDF. |
