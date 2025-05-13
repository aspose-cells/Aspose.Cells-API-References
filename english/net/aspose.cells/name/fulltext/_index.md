---
title: Name.FullText
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets the name full text of the object with the scope setting
type: docs
url: /net/aspose.cells/name/fulltext/
---
## Name.FullText property

Gets the name full text of the object with the scope setting.

```csharp
public string FullText { get; }
```

### Examples

```csharp
// Called: if (nm.FullText.Equals(reference))
public static Name Name_Property_FullText(NameCollection names, string reference)
        {
            if (reference.IndexOf('=') == 0)
            {
                reference = reference.Substring(1);
            }
            foreach (Name nm in names)
            {
                if (nm.FullText.Equals(reference))
                {
                    return nm;
                }
            }
            return null;
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


