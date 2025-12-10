---
title: Aspose::Cells::Drawing::PictureCollection::Add method
linktitle: Add
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::PictureCollection::Add method. Adds a picture to the collection in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.drawing/picturecollection/add/
---
## PictureCollection::Add(int32_t, int32_t, int32_t, int32_t, const Vector \<uint8_t\>\&) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const Vector<uint8_t> &stream)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| bottomRow | int32_t | Lower right row index |
| rightColumn | int32_t | Lower right column index |
| stream | const Vector \<uint8_t\>\& | Stream object which contains the image data. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//Get image data from file(e.g image.jpg)
//(Note: You need to read the data into this variable.)
Vector<uint8_t> fs{0};

//add a picture
int index = pictures.Add(1, 1, 5, 5, fs);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, int32_t, int32_t, const U16String\&) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const U16String &fileName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| bottomRow | int32_t | Lower right row index |
| rightColumn | int32_t | Lower right column index |
| fileName | const U16String\& | Image filename. |

## ReturnValue

[Picture](../../picture/) object index.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, int32_t, int32_t, const char16_t*) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const char16_t *fileName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| bottomRow | int32_t | Lower right row index |
| rightColumn | int32_t | Lower right column index |
| fileName | const char16_t* | Image filename. |

## ReturnValue

[Picture](../../picture/) object index.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, const Vector \<uint8_t\>\&) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, const Vector<uint8_t> &stream)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| stream | const Vector \<uint8_t\>\& | Stream object which contains the image data. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//Get image data from file(e.g image.jpg)
//(Note: You need to read the data into this variable.)
Vector<uint8_t> fs{ 0 };

//add a picture
pictures.Add(1, 1, fs);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, const U16String\&) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, const U16String &fileName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| fileName | const U16String\& | Image filename. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//add a picture
U16String imageFile = u"image.jpg";
pictures.Add(1, 1, imageFile);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, const char16_t*) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, const char16_t *fileName)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| fileName | const char16_t* | Image filename. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//add a picture
pictures.Add(1, 1, u"image.jpg");
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, const Vector \<uint8_t\>\&, int32_t, int32_t) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, const Vector<uint8_t> &stream, int32_t widthScale, int32_t heightScale)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| stream | const Vector \<uint8_t\>\& | Stream object which contains the image data. |
| widthScale | int32_t | Scale of image width, a percentage. |
| heightScale | int32_t | Scale of image height, a percentage. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//Get image data from file(e.g image.jpg)
//(Note: You need to read the data into this variable.)
Vector<uint8_t> fs{ 0 };

//add a picture
pictures.Add(1, 1, fs, 50, 50);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, const U16String\&, int32_t, int32_t) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, const U16String &fileName, int32_t widthScale, int32_t heightScale)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| fileName | const U16String\& | Image filename. |
| widthScale | int32_t | Scale of image width, a percentage. |
| heightScale | int32_t | Scale of image height, a percentage. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//add a picture
U16String imageFile = u"image.jpg";
pictures.Add(1, 1, imageFile, 50, 50);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## PictureCollection::Add(int32_t, int32_t, const char16_t*, int32_t, int32_t) method


Adds a picture to the collection.

```cpp
int32_t Aspose::Cells::Drawing::PictureCollection::Add(int32_t topRow, int32_t leftColumn, const char16_t *fileName, int32_t widthScale, int32_t heightScale)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| fileName | const char16_t* | Image filename. |
| widthScale | int32_t | Scale of image width, a percentage. |
| heightScale | int32_t | Scale of image height, a percentage. |

## ReturnValue

[Picture](../../picture/) object index.


## Examples


```cpp
//add a picture
pictures.Add(1, 1, u"image.jpg", 50, 50);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
