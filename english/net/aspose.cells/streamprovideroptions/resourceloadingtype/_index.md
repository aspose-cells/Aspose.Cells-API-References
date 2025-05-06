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
// Called: options.ResourceLoadingType = ResourceLoadingType.UserProvided;
public void Property_ResourceLoadingType(StreamProviderOptions options)
            {
                options.Stream = File.OpenRead(Constants.sourcePath + &quot;image1.png&quot;);
                options.ResourceLoadingType = ResourceLoadingType.UserProvided;
            }
```

### See Also

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


