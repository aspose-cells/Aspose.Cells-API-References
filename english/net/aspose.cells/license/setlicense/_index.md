---
title: License.SetLicense
second_title: Aspose.Cells for .NET API Reference
description: License method. Licenses the component
type: docs
url: /net/aspose.cells/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Licenses the component.

```csharp
public void SetLicense(string licenseName)
```

### Remarks

Tries to find the license in the following locations:

1. Explicit path.

2. The folder that contains the Aspose component assembly.

3. The folder that contains the client's calling assembly.

4. The folder that contains the entry (startup) assembly.

5. An embedded resource in the client's calling assembly.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Explicit path.

2. An embedded resource in the client's calling assembly.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodSetLicenseWithStringDemo
    {
        public static void Run()
        {
            License license = new License();
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### See Also

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetLicense(Stream) {#setlicense}

Licenses the component.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A stream that contains the license. |

### Remarks

Use this method to load a license from a stream.

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodSetLicenseWithStreamDemo
    {
        public static void Run()
        {
            // Create a memory stream with license file content
            byte[] licenseBytes = File.ReadAllBytes("Aspose.Cells.lic");
            using (MemoryStream myStream = new MemoryStream(licenseBytes))
            {
                License license = new License();
                license.SetLicense(myStream);
                Console.WriteLine("License set successfully.");
            }
        }
    }
}
```

### See Also

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


