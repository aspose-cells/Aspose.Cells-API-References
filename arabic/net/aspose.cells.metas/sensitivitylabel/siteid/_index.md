---
title: "SensitivityLabel.SiteId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SensitivityLabel property. يمثل معرف موقع Azure Active Directory (Azure AD) المتعلق بسياسة تسمية الحساسية التي تصف تسمية الحساسية"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

يمثل معرّف موقع Azure Active Directory (Azure AD) المتعلق بسياسة تسمية الحساسية التي تصف تسمية الحساسية.

```csharp
public string SiteId { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // إنشاء نسخة من SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));

                // تعيين الخصائص الأساسية
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;

                // أظهر الحصول على القيمة الأولية لـ SiteId
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // عيّن SiteId إلى معرف موقع Azure AD تجريبي
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // غيّر SiteId لتوضح أنها قابلة للقراءة والكتابة
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // أظهر كيف يرتبط SiteId بالخصائص الأخرى
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // احفظ المصنف
                workbook.Save("SiteIdDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


