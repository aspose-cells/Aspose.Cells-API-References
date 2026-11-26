---
title: "Класс VbaProject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Vba.VbaProject. Представляет VBA‑проект"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Представляет проект VBA.

```csharp
public class VbaProject
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Получает необработанные данные сертификата, если этот VBA‑проект подписан. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Получает и задаёт кодировку VBA‑проекта. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Указывает, заблокирован ли этот VBA‑проект для просмотра. Если true, код не будет виден. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolete.**) Указывает, заблокирован ли этот VBA‑проект для просмотра. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Указывает, защищён ли этот VBA‑проект. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Указывает, подписан ли VBAcode или нет. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Указывает, действительна ли подпись проекта VBA или нет. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Получает все объекты [`VbaModule`](../vbamodule/). |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Получает и задает имя проекта VBA. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Получает все ссылки проекта VBA. |

## Методы

| Имя | Описание |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Копирует проект VBA из другого файла. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Защищает или снимает защиту с этого проекта VBA. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Подписывает этот проект VBA цифровой подписью |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Проверяет пароль защиты. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Text;
    using System.Security.Cryptography.X509Certificates;

    public class VbaProjectDemo
    {
        public static void VbaProjectExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Установка свойств
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Проверка свойств только для чтения.
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Добавление модуля VBA.
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Добавление ссылки проекта VBA.
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Защита проекта VBA.
            vbaProject.Protect(true, "password");

            // Подписание проекта VBA.
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Сохранение файла Excel
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


