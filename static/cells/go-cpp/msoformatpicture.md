##MsoFormatPicture Class
'MsoFormatPicture class. Encapsulates the object that represents msoformatpicture in Go.'
## MsoFormatPicture class
Represents the picture format.
```go
type MsoFormatPicture struct  {
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
|[GetTopCropInch](./gettopcropinch/) | Represents the location of the top of the crop rectangle expressed, in unit of inches. |
|[SetTopCropInch](./settopcropinch/) | Represents the location of the top of the crop rectangle expressed, in unit of inches. |
|[GetBottomCropInch](./getbottomcropinch/) | Represents the location of the bottom of the crop rectangle expressed, in unit of inches. |
|[SetBottomCropInch](./setbottomcropinch/) | Represents the location of the bottom of the crop rectangle expressed, in unit of inches. |
|[GetLeftCropInch](./getleftcropinch/) | Represents the location of the left of the crop rectangle expressed, in unit of inches. |
|[SetLeftCropInch](./setleftcropinch/) | Represents the location of the left of the crop rectangle expressed, in unit of inches. |
|[GetRightCropInch](./getrightcropinch/) | Represents the location of the right of the crop rectangle expressed, in unit of inches. |
|[SetRightCropInch](./setrightcropinch/) | Represents the location of the right of the crop rectangle expressed, in unit of inches. |
|[GetTopCrop](./gettopcrop/) | Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height. |
|[SetTopCrop](./settopcrop/) | Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height. |
|[GetBottomCrop](./getbottomcrop/) | Represents the location of the bottom of the crop rectangle expressed, expressed as a ratio of the image's height. |
|[SetBottomCrop](./setbottomcrop/) | Represents the location of the bottom of the crop rectangle expressed, expressed as a ratio of the image's height. |
|[GetLeftCrop](./getleftcrop/) | Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width. |
|[SetLeftCrop](./setleftcrop/) | Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width. |
|[GetRightCrop](./getrightcrop/) | Represents the location of the right of the crop rectangle expressed, expressed as a ratio of the image's width. |
|[SetRightCrop](./setrightcrop/) | Represents the location of the right of the crop rectangle expressed, expressed as a ratio of the image's width. |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetTransparentColor](./gettransparentcolor/) | Gets and sets the transparent color of the picture. |
|[SetTransparentColor](./settransparentcolor/) | Gets and sets the transparent color of the picture. |
|[GetContrast](./getcontrast/) | Represents the contrast modification for the picture.in unit of percentage. |
|[SetContrast](./setcontrast/) | Represents the contrast modification for the picture.in unit of percentage. |
|[GetBrightness](./getbrightness/) | Represents the brightness modification for the picture in unit of percentage. |
|[SetBrightness](./setbrightness/) | Represents the brightness modification for the picture in unit of percentage. |
|[GetGamma](./getgamma/) | Represents gamma of the picture. |
|[SetGamma](./setgamma/) | Represents gamma of the picture. |
|[IsBiLevel](./isbilevel/) | Indicates whether this picture should display in two-color black and white. |
|[SetIsBiLevel](./setisbilevel/) | Indicates whether this picture should display in two-color black and white. |
|[IsGray](./isgray/) | Indicates whether this picture should display in grayscale. |
|[SetIsGray](./setisgray/) | Indicates whether this picture should display in grayscale. |
|[GetHashCode](./gethashcode/) | Gets the hash code. |
|[Equals](./equals/) |  |
