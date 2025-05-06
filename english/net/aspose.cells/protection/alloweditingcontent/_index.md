---
title: Protection.AllowEditingContent
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to edit contents of locked cells on a protected worksheet
type: docs
url: /net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

```csharp
public bool AllowEditingContent { get; set; }
```

### Examples

```csharp
// Called: sheet.Protection.AllowEditingContent = false;
[Test]
        // http://www.aspose.com/community/forums/thread/254918/lock-cells-not-working-with-version-4.9.1.0.aspx
        public void Property_AllowEditingContent()
        {
            Console.WriteLine(&quot;Property_AllowEditingContent()&quot;);
            string outfn = Constants.destPath + &quot;Test_StyleProtectionCellLock_out.xlsx&quot;;

            Workbook workbook = new Workbook();
            Aspose.Cells.Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells[0, 1].PutValue(&quot;Editable1&quot;);
            sheet.Cells[0, 2].PutValue(&quot;Editable2&quot;);

            Aspose.Cells.Style styleWorking = workbook.CreateStyle();
            styleWorking.IsLocked = false;
            styleWorking.Font.Color = System.Drawing.Color.Green;
            sheet.Cells[0, 1].SetStyle(styleWorking);

            Aspose.Cells.Style styleNotWorking = workbook.CreateStyle();
            styleNotWorking.IsLocked = false;
            styleNotWorking.Font.Color = System.Drawing.Color.Red;
            styleNotWorking.Name = &quot;EditableCell&quot;;
            sheet.Cells[0, 2].SetStyle(styleNotWorking);

            sheet.Protection.AllowEditingContent = false;

            workbook.Save(outfn);

            workbook = new Workbook(outfn);
            Cells cells = workbook.Worksheets[0].Cells;
            Cell c1 = cells[0, 1];
            Cell c2 = cells[0, 2];

            //if(c2.Style.IsLocked)
            //  throw new Exception(&quot;Property_AllowEditingContent() failed!&quot;);
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


