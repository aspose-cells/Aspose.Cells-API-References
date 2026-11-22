---
title: "الفئة VbaProject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Vba.VbaProject. تمثل مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

يمثل مشروع VBA.

```csharp
public class VbaProject
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | يحصل على البيانات الأولية للشهادة إذا كان مشروع VBA هذا موقعًا. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | يحصل ويضبط ترميز مشروع VBA. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | يشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض. إذا كان صحيحًا، لا يمكن رؤية الشيفرات. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**مهمل.**) يشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | يشير إلى ما إذا كان مشروع VBA هذا محميًا. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | يشير إلى ما إذا كان VBAcode موقعًا أم لا. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | يشير إلى ما إذا كانت توقيع مشروع VBA صالحًا أم لا. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | يحصل على جميع كائنات [`VbaModule`](../vbamodule/). |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | يحصل على اسم مشروع VBA ويضبطه. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | يحصل على جميع مراجع مشروع VBA. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | نسخ مشروع VBA من ملف آخر. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | يحمي أو يزيل الحماية عن مشروع VBA هذا. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | وقّع مشروع VBA هذا باستخدام DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | يتحقق من صحة كلمة مرور الحماية. |

### أمثلة

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
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;

            // ضبط الخصائص
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // التحقق من الخصائص للقراءة فقط
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // إضافة وحدة VBA
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // إضافة مرجع مشروع VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // حماية مشروع VBA
            vbaProject.Protect(true, "password");

            // توقيع مشروع VBA
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // حفظ ملف Excel
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


