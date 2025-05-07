---
title: StreamProviderOptions.ResourceLoadingType
second_title: Aspose.Cells for .NET API Reference
description: StreamProviderOptions property. Gets and sets the type of loading resource
type: docs
url: /net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Gets and sets the type of loading resource.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Examples

```csharp
// Called: if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
public void Property_ResourceLoadingType(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Provide a custom stream for the resource
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Skip loading the resource
                options.Stream = Stream.Null;
            }
            else
            {
                // Load the resource as usual
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }
```

### See Also

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


