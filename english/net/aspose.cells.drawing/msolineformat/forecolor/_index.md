---
title: MsoLineFormat.ForeColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Gets and sets the border line fore color
type: docs
url: /net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

Gets and sets the border line fore color.

```csharp
public Color ForeColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(commentSrc.CommentShape.LineFormat.ForeColor, commentDest.CommentShape.LineFormat.ForeColor, info + &amp;quot;.CommentShape.LineFormat.ForeColor&amp;quot;);
public static void Property_ForeColor(Comment commentSrc, Comment commentDest, string info)
        {           
            if (AssertHelper.checkNull(commentSrc, commentDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(commentSrc.IsVisible, commentDest.IsVisible, info + &quot;.IsVisible&quot;);
            //============Properties be supported in excel 2003 format file===================//
            if (commentSrc.IsVisible &amp;&amp; commentDest.IsVisible)
            {
                AssertHelper.AreEqual(commentSrc.Row, commentDest.Row, info + &quot;.Row&quot;);
                AssertHelper.AreEqual(commentSrc.Column, commentDest.Column, info + &quot;.Column&quot;);
                AssertHelper.AreEqual(commentSrc.Note, commentDest.Note, info + &quot;.Note&quot;);
                CharactersTest.Property_ForeColor(commentSrc.GetRichFormattings(), commentDest.GetRichFormattings(), info + &quot;.GetCharacters()&quot;);
                //===Font====//
                FontTest.Property_ForeColor(commentSrc.Font, commentDest.Font, info + &quot;.Font&quot;);
                //===alignment====//
                AssertHelper.AreEqual(commentSrc.TextHorizontalAlignment, commentDest.TextHorizontalAlignment, info + &quot;.TextHorizontalAlignment&quot;);
                AssertHelper.AreEqual(commentSrc.TextVerticalAlignment, commentDest.TextVerticalAlignment, info + &quot;.TextVerticalAlignment&quot;);
                AssertHelper.AreEqual(commentSrc.TextOrientationType, commentDest.TextOrientationType, info + &quot;.TextOrientationType&quot;);
                AssertHelper.AreEqual(commentSrc.AutoSize, commentDest.AutoSize, info + &quot;.AutoSize&quot;);                
                //remark:ȱ��TextDirectionType 
                //===colors and lines===//
                AssertHelper.AreEqual(commentSrc.CommentShape.FillFormat.IsVisible, commentDest.CommentShape.FillFormat.IsVisible, info + &quot;.CommentShape.FillFormat.IsVisible&quot;);
                if (commentSrc.CommentShape.FillFormat.IsVisible &amp;&amp; commentDest.CommentShape.FillFormat.IsVisible)
                {
                    AssertHelper.Property_ForeColor(commentSrc.CommentShape.FillFormat.ForeColor, commentDest.CommentShape.FillFormat.ForeColor, info + &quot;.CommentShape.FillFormat.ForeColor&quot;);
                    AssertHelper.Property_ForeColor(commentSrc.CommentShape.FillFormat.BackColor, commentDest.CommentShape.FillFormat.BackColor, info + &quot;.CommentShape.FillFormat.BackColor&quot;);
                    AssertHelper.AreEqual(commentSrc.CommentShape.FillFormat.Transparency, commentDest.CommentShape.FillFormat.Transparency, info + &quot;.CommentShape.FillFormat.Transparency&quot;);
                }
                AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.IsVisible, commentDest.CommentShape.LineFormat.IsVisible, info + &quot;.CommentShape.LineFormat.IsVisible&quot;);
                if (commentSrc.CommentShape.LineFormat.IsVisible &amp;&amp; commentDest.CommentShape.LineFormat.IsVisible)
                {                    
                    AssertHelper.Property_ForeColor(commentSrc.CommentShape.LineFormat.ForeColor, commentDest.CommentShape.LineFormat.ForeColor, info + &quot;.CommentShape.LineFormat.ForeColor&quot;);
                    AssertHelper.Property_ForeColor(commentSrc.CommentShape.LineFormat.BackColor, commentDest.CommentShape.LineFormat.BackColor, info + &quot;.CommentShape.LineFormat.BackColor&quot;);
                    AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.Style, commentDest.CommentShape.LineFormat.Style, info + &quot;.CommentShape.LineFormat.Style&quot;);
                    AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.DashStyle, commentDest.CommentShape.LineFormat.DashStyle, info + &quot;.CommentShape.LineFormat.DashStyle&quot;);
                    AssertHelper.AreEqual(commentSrc.CommentShape.LineFormat.Weight, commentDest.CommentShape.LineFormat.Weight, info + &quot;.CommentShape.LineFormat.Weight&quot;);                    
                }
                //===size====//
                AssertHelper.AreEqual(commentSrc.CommentShape.HeightCM, commentDest.CommentShape.HeightCM, info + &quot;.CommentShape.HeightCM&quot;);
                AssertHelper.AreEqual(commentSrc.CommentShape.WidthCM, commentDest.CommentShape.WidthCM, info + &quot;.CommentShape.WidthCM&quot;);
                AssertHelper.AreEqual(commentSrc.CommentShape.HeightScale, commentDest.CommentShape.HeightScale, info + &quot;.CommentShape.HeightScale&quot;);
                AssertHelper.AreEqual(commentSrc.CommentShape.WidthScale, commentDest.CommentShape.WidthScale, info + &quot;.CommentShape.WidthScale&quot;);
                AssertHelper.AreEqual(commentSrc.CommentShape.IsLockAspectRatio, commentDest.CommentShape.IsLockAspectRatio, info + &quot;.CommentShape.IsLockAspectRatio&quot;);
                //===protection====//
                AssertHelper.AreEqual(commentSrc.CommentShape.IsLocked, commentDest.CommentShape.IsLocked, info + &quot;.CommentShape.IsLocked&quot;);
                //ȱ��IsLockText              
                //===properties===//
                AssertHelper.AreEqual(commentSrc.CommentShape.Placement, commentDest.CommentShape.Placement, info + &quot;.CommentShape.Placement&quot;);
                //===margins=====//
                TextFrameTest.Property_ForeColor(commentSrc.CommentShape.TextBody.TextAlignment, commentDest.CommentShape.TextBody.TextAlignment, info+&quot;.CommentShape.TextFrame&quot;);    
                //===Web====//
                AssertHelper.AreEqual(commentSrc.CommentShape.AlternativeText, commentDest.CommentShape.AlternativeText, info + &quot;.CommentShape.AlternativeText&quot;);
                //other                 
                HyperlinksTest.Property_ForeColor(commentSrc.CommentShape.Hyperlink, commentDest.CommentShape.Hyperlink, info + &quot;.CommentShape.Hyperlink&quot;);

                AssertHelper.AreEqual(commentSrc.HtmlNote, commentDest.HtmlNote, info + &quot;.HtmlNote&quot;);
            }               
        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


