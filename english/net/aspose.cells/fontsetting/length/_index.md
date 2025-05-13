---
title: FontSetting.Length
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Gets the length of the characters
type: docs
url: /net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Gets the length of the characters.

```csharp
public int Length { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(arrcharSrc.Length, arrcharDest.Length, info + ".Length");
public static void FontSetting_Property_Length(FontSetting arrcharSrc, FontSetting arrcharDest, string info)
        {            
            AssertHelper.AreEqual(arrcharSrc.StartIndex, arrcharDest.StartIndex, info + ".StartIndex");
            AssertHelper.AreEqual(arrcharSrc.Length, arrcharDest.Length, info + ".Length");
            FontTest.FontSetting_Property_Length(arrcharSrc.Font, arrcharDest.Font, info + ".Font");
        }
```

### See Also

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


