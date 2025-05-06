---
title: OleObject.SourceFullName
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Returns the source full name of the source file for the linked OLE object
type: docs
url: /net/aspose.cells.drawing/oleobject/sourcefullname/
---
## OleObject.SourceFullName property

Returns the source full name of the source file for the linked OLE object.

```csharp
[Obsolete("Use OleObject.ObjectSourceFullName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SourceFullName { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use OleObject.ObjectSourceFullName property. This property will be removed 12 months later since November 2013. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: FileStream outOleFs = new FileStream(path + o.SourceFullName, FileMode.OpenOrCreate);
public void Property_SourceFullName()
        {
            string infn = path + &quot;TEST_OLE_Book1.xlsx&quot;;
            string outfn = Constants.destPath + &quot;TEST_OLE_Book1_out.xlsx&quot;;
            Workbook book = new Workbook();
            book= new Workbook(infn);
            OleObjectCollection os = book.Worksheets[0].OleObjects;
            for (int i = 0; i &lt; os.Count; i++)
            {
                OleObject o = os[i];
                FileStream outOleFs = new FileStream(path + o.SourceFullName, FileMode.OpenOrCreate);
                outOleFs.Write(o.ObjectData, 0, o.ObjectData.Length);
                outOleFs.Close();
            }
            book.Save(outfn);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


