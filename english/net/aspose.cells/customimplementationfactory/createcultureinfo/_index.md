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
// Called: CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
public static void CustomImplementationFactory_Method_CreateCultureInfo()
        {
            // Create an instance of CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrate the CreateMemoryStream method without parameters
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Demonstrate the CreateMemoryStream method with capacity parameter
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Demonstrate the CreateCultureInfo method
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Demonstrate the CreateRandomInstance method
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Example usage of the factory with CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


