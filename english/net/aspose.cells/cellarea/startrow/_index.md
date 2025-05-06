---
title: CellArea.StartRow
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the start row of this area
type: docs
url: /net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Gets or set the start row of this area.

```csharp
public int StartRow;
```

### Examples

```csharp
// Called: if (cellarea.StartRow == 4 &amp;amp;&amp;amp; cellarea.EndRow == 4 &amp;amp;&amp;amp; cellarea.StartColumn == 0 &amp;amp;&amp;amp; cellarea.EndColumn == 0)
public void Field_StartRow(CellArea cellarea, Validation validation)
        {
            if (cellarea.StartRow == 4 &amp;&amp; cellarea.EndRow == 4 &amp;&amp; cellarea.StartColumn == 0 &amp;&amp; cellarea.EndColumn == 0)
            {
                ReflectInvoker.invoke(&quot;validation&quot;, validation, new Object[][]{
				    new Object[]{&quot;Type&quot;, ValidationType.Decimal},
				    new Object[]{&quot;Operator&quot;, OperatorType.NotBetween},
				    new Object[]{&quot;IgnoreBlank&quot;, true},
				    new Object[]{&quot;Formula1&quot;, &quot;=A1&quot;},
				    new Object[]{&quot;Formula2&quot;, &quot;=A2&quot;},               
				    new Object[]{&quot;ShowInput&quot;, true},				
				    new Object[]{&quot;ShowError&quot;, true},
				    new Object[]{&quot;AlertStyle&quot;, ValidationAlertType.Stop}});
            }
            else if (cellarea.StartRow == 2 &amp;&amp; cellarea.EndRow == 2 &amp;&amp; cellarea.StartColumn == 2 &amp;&amp; cellarea.EndColumn == 2)
            {
                ReflectInvoker.invoke(&quot;validation&quot;, validation, new Object[][]{
				    new Object[]{&quot;Type&quot;, ValidationType.TextLength},
				    new Object[]{&quot;Operator&quot;, OperatorType.Equal},
				    new Object[]{&quot;IgnoreBlank&quot;, false},
				    new Object[]{&quot;Formula1&quot;, &quot;=7&quot;},
				    new Object[]{&quot;ShowInput&quot;, true},
				    new Object[]{&quot;InputTitle&quot;, &quot;title test&quot;},
				    new Object[]{&quot;InputMessage&quot;, &quot;message test&quot;},
				    new Object[]{&quot;ShowError&quot;, true},
				    new Object[]{&quot;AlertStyle&quot;, ValidationAlertType.Warning},
				    new Object[]{&quot;ErrorTitle&quot;, &quot;title1&quot;},
				    new Object[]{&quot;ErrorMessage&quot;, &quot;error&quot;}});       
            }
            else if (cellarea.StartRow == 0 &amp;&amp; cellarea.EndRow == 0 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp; cellarea.EndColumn == 5)
            {
                ReflectInvoker.invoke(&quot;validation&quot;, validation, new Object[][]{
				    new Object[]{&quot;Type&quot;, ValidationType.List},
                    new Object[]{&quot;IgnoreBlank&quot;, true}, 
                    new Object[]{&quot;InCellDropDown&quot;, true},
                    new Object[]{&quot;Formula1&quot;, &quot;=$E$1:$E$5&quot;},
                    new Object[]{&quot;ShowInput&quot;, false},
                    new Object[]{&quot;ShowError&quot;, false}
                  });
            }
            else if (cellarea.StartRow == 14 &amp;&amp; cellarea.EndRow == 17 &amp;&amp; cellarea.StartColumn == 4 &amp;&amp; cellarea.EndColumn == 4)
            {               
                ReflectInvoker.invoke(&quot;validation&quot;, validation, new Object[][]{
                    new Object[]{&quot;Type&quot;, ValidationType.Custom},
                    new Object[]{&quot;IgnoreBlank&quot;, true},              
                    new Object[]{&quot;Formula1&quot;, &quot;=SUM(E15:E18)&quot;},
                    new Object[]{&quot;ShowInput&quot;, false},
                    new Object[]{&quot;ShowError&quot;, false}
                  });
            }

        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


