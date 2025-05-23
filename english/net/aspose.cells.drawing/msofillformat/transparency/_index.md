---
title: MsoFillFormat.Transparency
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Returns or sets the degree of transparency of the specified fill as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(commentSrc.CommentShape.FillFormat.Transparency, commentDest.CommentShape.FillFormat.Transparency, info + ".CommentShape.FillFormat.Transparency");
public static void MsoFillFormat_Property_Transparency(Comment commentSrc, Comment commentDest, string info)
        {           
            if (AssertHelper.checkNull(commentSrc, commentDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(commentSrc.IsVisible, commentDest.IsVisible, info + ".IsVisible");
            //============Properties be supported in excel 2003 format file===================//
            if (commentSrc.IsVisible && commentDest.IsVisible)
            {
                AssertHelper.AreEqual(commentSrc.Row, commentDest.Row, info + ".Row");
                AssertHelper.AreEqual(commentSrc.Column, commentDest.Column, info + ".Column");
                AssertHelper.AreEqual(commentSrc.Note, commentDest.Note, info + ".Note");
                CharactersTest.MsoFillFormat_Property_Transparency(commentSrc.GetRichFormattings(), commentDest.GetRichFormattings(), info + ".GetCharacters()");
                //===Font====//
                FontTest.MsoFillFormat_Property_Transparency(commentSrc.Font, commentDest.Font, info + ".Font");
                //===alignment====//
                AssertHelper.AreEqual(commentSrc.TextHorizontalAlignment, commentDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
                AssertHelper.AreEqual(commentSrc.TextVerticalAlignment, commentDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
                AssertHelper.AreEqual(commentSrc.TextOrientationType, commentDest.TextOrientationType, info + ".TextOrientationType");
                AssertHelper.AreEqual(commentSrc.AutoSize, commentDest.AutoSize, info + ".AutoSize");                
                //remark:ȱ��TextDirectionType 
                //===colors and lines===//
                AssertHelper.AreEqual(commentSrc.CommentShape.FillFormat.IsVisible, commentDest.CommentShape.FillFormat.IsVisible, info + ".CommentShape.FillFormat.IsVisible");
                if (commentSrc.CommentShape.FillFormat.IsVisible && commentDest.CommentShape.FillFormat.IsVisible)
                {
                    AssertHelper.MsoFillFormat_Property_Transparency(commentSrc.CommentShape.FillFormat.ForeColor, commentDest.CommentShape.FillFormat.ForeColor, info + ".CommentShape.FillFormat.ForeColor");
                    AssertHelper.MsoFillFormat_Property_Transparency(commentSrc.CommentShape.FillFormat.BackColor, commentDest.CommentShape.FillFormat.BackColor, info + ".CommentShape.FillFormat.BackColor");
                    AssertHelper.AreEqual(commentSrc.CommentShape.FillFormat.Transparency, commentDest.CommentShape.FillFormat.Transparency, info + ".CommentShape.FillFormat.Transparency");
                }
                AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.IsVisible, commentDest.CommentShape.LineFormat.IsVisible, info + ".CommentShape.LineFormat.IsVisible");
                if (commentSrc.CommentShape.LineFormat.IsVisible && commentDest.CommentShape.LineFormat.IsVisible)
                {                    
                    AssertHelper.MsoFillFormat_Property_Transparency(commentSrc.CommentShape.LineFormat.ForeColor, commentDest.CommentShape.LineFormat.ForeColor, info + ".CommentShape.LineFormat.ForeColor");
                    AssertHelper.MsoFillFormat_Property_Transparency(commentSrc.CommentShape.LineFormat.BackColor, commentDest.CommentShape.LineFormat.BackColor, info + ".CommentShape.LineFormat.BackColor");
                    AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.Style, commentDest.CommentShape.LineFormat.Style, info + ".CommentShape.LineFormat.Style");
                    AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.DashStyle, commentDest.CommentShape.LineFormat.DashStyle, info + ".CommentShape.LineFormat.DashStyle");
                    AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.Weight, commentDest.CommentShape.LineFormat.Weight, info + ".CommentShape.LineFormat.Weight");                    
                }
                //===size====//
                AssertHelper.AreEqual(commentSrc.CommentShape.HeightCM, commentDest.CommentShape.HeightCM, info + ".CommentShape.HeightCM");
                AssertHelper.AreEqual(commentSrc.CommentShape.WidthCM, commentDest.CommentShape.WidthCM, info + ".CommentShape.WidthCM");
                AssertHelper.AreEqual(commentSrc.CommentShape.HeightScale, commentDest.CommentShape.HeightScale, info + ".CommentShape.HeightScale");
                AssertHelper.AreEqual(commentSrc.CommentShape.WidthScale, commentDest.CommentShape.WidthScale, info + ".CommentShape.WidthScale");
                AssertHelper.AreEqual(commentSrc.CommentShape.IsLockAspectRatio, commentDest.CommentShape.IsLockAspectRatio, info + ".CommentShape.IsLockAspectRatio");
                //===protection====//
                AssertHelper.AreEqual(commentSrc.CommentShape.IsLocked, commentDest.CommentShape.IsLocked, info + ".CommentShape.IsLocked");
                //ȱ��IsLockText              
                //===properties===//
                AssertHelper.AreEqual(commentSrc.CommentShape.Placement, commentDest.CommentShape.Placement, info + ".CommentShape.Placement");
                //===margins=====//
                TextFrameTest.MsoFillFormat_Property_Transparency(commentSrc.CommentShape.TextBody.TextAlignment, commentDest.CommentShape.TextBody.TextAlignment, info+".CommentShape.TextFrame");    
                //===Web====//
                AssertHelper.AreEqual(commentSrc.CommentShape.AlternativeText, commentDest.CommentShape.AlternativeText, info + ".CommentShape.AlternativeText");
                //other                 
                HyperlinksTest.MsoFillFormat_Property_Transparency(commentSrc.CommentShape.Hyperlink, commentDest.CommentShape.Hyperlink, info + ".CommentShape.Hyperlink");

                AssertHelper.AreEqual(commentSrc.HtmlNote, commentDest.HtmlNote, info + ".HtmlNote");
            }               
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


