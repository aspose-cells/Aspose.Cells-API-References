---
title: CellsHelper.GetVersion
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Get the release version
type: docs
url: /net/aspose.cells/cellshelper/getversion/
---
## CellsHelper.GetVersion method

Get the release version.

```csharp
public static string GetVersion()
```

### Return Value

The release version.

### Examples

```csharp
// Called: Assert.AreEqual(pp[1], Aspose.Cells.CellsHelper.GetVersion());
public void Method_GetVersion()
        {
            string p = System.AppDomain.CurrentDomain.BaseDirectory;
            Assembly assembly = Assembly.LoadFile(p + @&quot;\Aspose.Cells.dll&quot;);
            string fullName = assembly.FullName;
            string[] ps = fullName.Split(&apos;,&apos;);
            Console.WriteLine(fullName);
            for (int i = 0; i &lt; ps.Length; i++)
            {
                ps[i] = ps[i].Trim();
                Console.WriteLine(ps[i]);
                if (ps[i].IndexOf(&apos;=&apos;) != -1)
                {
                    string[] pp = ps[i].Split(&apos;=&apos;);
                    switch (pp[0])
                    {
                        case &quot;Version&quot;:
                            Assert.AreEqual(pp[1], Aspose.Cells.CellsHelper.GetVersion());
                            Console.WriteLine(pp[1]);
                            break;
                        case &quot;PublicKeyToken&quot;:
                            Assert.AreEqual(pp[1], &quot;716fcc553a201e56&quot;);
                            Console.WriteLine(pp[1]);
                            break;
                    }
                }
                else
                {
                    Assert.AreEqual(ps[i], &quot;Aspose.Cells&quot;);
                }
            }
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


