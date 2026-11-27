---
title: "FileFormatUtil.VerifyPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Upptäcker och returnerar information om formatet för en Excel som lagras i en ström"
type: docs
url: /sv/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Detekterar och returnerar information om ett Excel-format som lagras i en ström.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström |  |
| lösenord | String | Lösenordet för krypterade ooxml‑filer. |

### Returvärde

Returnerar om lösenordet är korrekt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodVerifyPasswordWithStreamStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            string correctPassword = "test";
            string wrongPassword = "1234";

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, correctPassword);
                Console.WriteLine($"Password '{correctPassword}' is valid: {isValid}");
            }

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, wrongPassword);
                Console.WriteLine($"Password '{wrongPassword}' is valid: {isValid}");
            }
        }
    }
}
```

### Se även

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


