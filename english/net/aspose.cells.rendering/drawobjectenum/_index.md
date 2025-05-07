---
title: Enum DrawObjectEnum
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.DrawObjectEnum enum. Indicate Cell or Image of DrawObject
type: docs
url: /net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Indicate Cell or Image of DrawObject.

```csharp
public enum DrawObjectEnum
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Image | `0` | Indicate DrawObject is an Image |
| Cell | `1` | indicate DrawObject is an Cell |

### Examples

```csharp
// Called: if (drawObject.Type == DrawObjectEnum.Cell)
public override void Type_DrawObjectEnum(DrawObject drawObject, float x, float y,
                float width, float height)
            {
                // NOTE: All float coordinates *seem* to be in POINTS - 
                //   but JavaDoc doesn't specify.

                if (drawObject.Type == DrawObjectEnum.Cell)
                {
                    Cell cell = drawObject.Cell;

                    //check cell A1
                    if (cell.Row == 0 && cell.Column == 0)
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

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


