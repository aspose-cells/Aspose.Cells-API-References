---
title: ReferredArea.ToString
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea method. Returns the reference address of this area. Generally it is the address of the reference which may be used in formula such as Sheet1A1C3
type: docs
url: /net/aspose.cells/referredarea/tostring/
---
## ReferredArea.ToString method

Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".

```csharp
public override string ToString()
```

### Return Value

the reference address of this area.

### Examples

```csharp
// Called: Console.WriteLine(ra.ToString());
private void ReferredArea_Method_ToString(object v)
        {
            if (v == null)
            {
                Console.WriteLine("null");
            }
            else if (v is object[])
            {
                Console.Write("{");
                object[] vs = (object[])v;
                foreach (object vo in vs)
                {
                    Console.Write(vo + ",");
                }
                Console.WriteLine("}");
            }
            else if (v is ReferredArea)
            {
                ReferredArea ra = (ReferredArea)v;
                Console.WriteLine(ra.ToString());
            }
            else
            {
                Console.WriteLine(v);
            }
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


