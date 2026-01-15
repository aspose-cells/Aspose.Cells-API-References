---
title: CustomImplementationFactory.CreateCultureInfo
second_title: Aspose.Cells for .NET API Reference
description: CustomImplementationFactory method. Create one CultureInfo by given id
type: docs
url: /net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Create one CultureInfo by given id.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| lcid | Int32 |  |

### Return Value

The CultureInfo instance.

### Remarks

This implementation is useful for situations: 1. Some cultures may not be supported by user's environment and creating the required CultureInfo with given identifier may cause Exception. To avoid the exception, user may override this method to provide a valid CultureInfo instance for the unsupported one. 2. User may want to specify some custom properties for some cultures to get expected result for formatting. For this purpose user may override this method to provide the CultureInfo instance with user specified properties. Please note UseUserOverride property of the returned CultureInfo instance may influence the formatted result. If it is false, some properties of the returned CultureInfo instance may be overridden by our built-in formatting engine according to the formatting requirements of different scenarios. If it is true, we will not change any properties of it and use it to format values directly. So, if user has specified custom properties for the returned CultureInfo instance, please make sure its UseUserOverride is true.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Call CreateCultureInfo with a valid LCID (1033 for English - United States)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Display the results
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Demonstrate setting the factory in CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


