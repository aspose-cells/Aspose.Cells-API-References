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
// Called: AssertHelper.AreEqual(arrcharSrc.Length, arrcharDest.Length, info + &amp;quot;.Length&amp;quot;);
public static void Property_Length(FontSetting arrcharSrc, FontSetting arrcharDest, string info)
        {            
            AssertHelper.AreEqual(arrcharSrc.StartIndex, arrcharDest.StartIndex, info + &quot;.StartIndex&quot;);
            AssertHelper.AreEqual(arrcharSrc.Length, arrcharDest.Length, info + &quot;.Length&quot;);
            FontTest.Property_Length(arrcharSrc.Font, arrcharDest.Font, info + &quot;.Font&quot;);
        }
```

### See Also

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


