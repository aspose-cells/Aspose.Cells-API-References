---
title: "CellsHelper.IsCloudPlatform"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابية مثل Azure أو AWSLambda وغيرها"
type: docs
url: /ar/net/aspose.cells/cellshelper/iscloudplatform/
---
## CellsHelper.IsCloudPlatform property

يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابة، مثل: Azure، AWSLambda، إلخ،

```csharp
public static bool IsCloudPlatform { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyIsCloudPlatformDemo
    {
        public static void Run()
        {
            // عيّن خاصية IsCloudPlatform
            CellsHelper.IsCloudPlatform = true;

            // أظهر استخدام الخاصية
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // أظهر كيف يؤثر ذلك على عمليات أخرى (مثال)
            if (CellsHelper.IsCloudPlatform)
            {
                Console.WriteLine("Running in cloud environment - using cloud-specific settings");
                CellsHelper.StartupPath = "/cloud_storage/aspose/cells";
            }
            else
            {
                Console.WriteLine("Running in local environment");
                CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


