---
title: Shape.ToImage
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Creates the shape image and saves it to a stream in the specified format
type: docs
url: /net/aspose.cells.drawing/shape/toimage/
---
## ToImage(Stream, ImageFormat) {#toimage_3}

Creates the shape image and saves it to a stream in the specified format.

```csharp
[Obsolete("Use Shape.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| imageFormat | ImageFormat | The format in which to save the image. |

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.ToImage(Stream, ImageType) method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_1}

Creates the shape image and saves it to a stream in the specified format.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| imageType | ImageType | The type in which to save the image. |

### Remarks

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### Examples

```csharp

[C#]
MemoryStream imageStream = new MemoryStream();
shape.ToImage(imageStream, ImageType.Png);
```

### See Also

* enum [ImageType](../../imagetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_4}

Saves the shape to a file.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

### Examples

```csharp

[C#]
ImageOrPrintOptions op = new ImageOrPrintOptions();
shape.ToImage("exmaple.png", op);
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_2}

Saves the shape to a stream.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

### Examples

```csharp

[C#]
MemoryStream imageStream = new MemoryStream();
ImageOrPrintOptions op = new ImageOrPrintOptions();
shape.ToImage(imageStream, op);
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage}

Returns the bitmap object of the shape .

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

### Examples

```csharp

[C#]
ImageOrPrintOptions op = new ImageOrPrintOptions();
System.Drawing.Bitmap btm = shape.ToImage(op);
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


