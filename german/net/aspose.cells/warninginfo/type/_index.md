---
title: "WarningInfo.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WarningInfo-Eigenschaft. Warnungstyp abrufen"
type: docs
url: /de/net/aspose.cells/warninginfo/type/
---
## WarningInfo.Type property

Warnungstyp abrufen.

```csharp
public ExceptionType Type { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyTypeDemo
    {
        private class CustomWarningCallback : IWarningCallback
        {
            public void Warning(WarningInfo warningInfo)
            {
                if (warningInfo.Type == ExceptionType.DefinedName)
                {
                    warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                    Console.WriteLine($"Corrected object: {warningInfo.CorrectedObject}");
                }
            }
        }

        public static void Run()
        {
            using (var workbook = new Workbook())
            {
                workbook.Worksheets.Add("Sheet1");
                int nameIndex = workbook.Worksheets.Names.Add("TestName");
                Name name = workbook.Worksheets.Names[nameIndex];
                name.RefersTo = "=Sheet1!$A$1";
                
                using (var stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    var loadOptions = new LoadOptions { WarningCallback = new CustomWarningCallback() };
                    new Workbook(stream, loadOptions);
                }
            }
        }
    }
}
```

### Siehe auch

* enum [ExceptionType](../../exceptiontype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


