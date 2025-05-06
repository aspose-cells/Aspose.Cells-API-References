---
title: Name.Text
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets the name text of the object
type: docs
url: /net/aspose.cells/name/text/
---
## Name.Text property

Gets the name text of the object.

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: string name = nameSrc.Text;
public static void Property_Text(NameCollection namesSrc, NameCollection namesDest, string info)
        {
            if (AssertHelper.checkNull(namesSrc, namesDest, info))
            {
                return;
            }
            int countSrc = namesSrc.Count;
            int countDest = namesDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + &quot;.Count&quot;);
            bool[] checkFlag = new bool[countDest];
            int countChecked = 0;
            for (int i = 0; i &lt; countSrc; i++)
            {
                Name nameSrc = namesSrc[i];
                string name = nameSrc.Text;
                Name nameDest = namesDest[i];

                Property_Text(nameSrc, nameDest, info + &quot;[&quot; + name + &quot;]&quot;);
            }
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


