---
title: DrawObject.Type
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the type of DrawObject
type: docs
url: /net/aspose.cells.rendering/drawobject/type/
---
## DrawObject.Type property

Indicates the type of DrawObject.

```csharp
public DrawObjectEnum Type { get; }
```

### Examples

```csharp
// Called: if (drawObject.Type == DrawObjectEnum.Cell)
public override void Property_Type(DrawObject drawObject, float x, float y,
                float width, float height)
            {
                // NOTE: All float coordinates *seem* to be in POINTS - 
                //   but JavaDoc doesn&apos;t specify.

                if (drawObject.Type == DrawObjectEnum.Cell)
                {
                    Cell cell = drawObject.Cell;

                    //check cell A1
                    if (cell.Row == 0 &amp;&amp; cell.Column == 0)
                    {
                        Assert.AreEqual(mPageIndex, drawObject.CurrentPage);

                        if (!mIsCached)
                        {
                            mX = x;
                            mY = y;
                            mWidth = width;
                            mHeight = height;
                        }
                        else
                        {
                            Assert.IsTrue(IsFloatEqual(mX, x));
                            Assert.IsTrue(IsFloatEqual(mY, y));
                            Assert.IsTrue(IsFloatEqual(mWidth, width));
                            Assert.IsTrue(IsFloatEqual(mHeight, height));

                        }
                    }
                }
            }
```

### See Also

* enum [DrawObjectEnum](../../drawobjectenum/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


