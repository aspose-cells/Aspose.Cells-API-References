---
title: FontSetting.StartIndex
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Gets the start index of the characters
type: docs
url: /net/aspose.cells/fontsetting/startindex/
---
## FontSetting.StartIndex property

Gets the start index of the characters.

```csharp
public int StartIndex { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(arrcharSrc.StartIndex, arrcharDest.StartIndex, info + ".StartIndex");
public static void Property_StartIndex(FontSetting arrcharSrc, FontSetting arrcharDest, string info)
        {            
            AssertHelper.AreEqual(arrcharSrc.StartIndex, arrcharDest.StartIndex, info + ".StartIndex");
            AssertHelper.AreEqual(arrcharSrc.Length, arrcharDest.Length, info + ".Length");
            FontTest.Property_StartIndex(arrcharSrc.Font, arrcharDest.Font, info + ".Font");
        }
```

### See Also

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


