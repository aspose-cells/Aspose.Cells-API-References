##FontSettingCollection Class
'FontSettingCollection class. Encapsulates the object that represents fontsettingcollection in Go.'
## FontSettingCollection class
Represents the list of <see cref="FontSetting"/>.
```go
type FontSettingCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[SetWordArtStyle](./setwordartstyle/) | Sets the preset WordArt style. |
|[GetTextAlignment](./gettextalignment/) | Represents the alignment setting of the text body. |
|[GetTextParagraphs](./gettextparagraphs/) | Gets all paragraphs. |
|[GetParagraphEnumerator](./getparagraphenumerator/) | Gets the enumerator of the paragraphs. |
|[GetText](./gettext/) | Gets and sets the text of the shape. |
|[SetText](./settext/) | Gets and sets the text of the shape. |
|[AppendText](./appendtext/) | Appends the text. |
|[InsertText](./inserttext/) | Insert index at the position. |
|[Replace_Int_Int_String](./replace_int_int_string/) | Replace the text. |
|[Replace_String_String](./replace_string_string/) | Replace the text. |
|[DeleteText](./deletetext/) | Delete some characters. |
|[GetHtmlString](./gethtmlstring/) | Gets and sets the html string which contains data and some formats in this shape. |
|[SetHtmlString](./sethtmlstring/) | Gets and sets the html string which contains data and some formats in this shape. |
|[Format](./format/) | Format the text with font setting. |
|[Get](./get/) | Gets the FontSetting by the index. |
|[Clear](./clear/) | Clear all setting. |
|[Equals](./equals/) |  |
|[GetHashCode](./gethashcode/) |  |
|[GetCount](./getcount/) |  |
