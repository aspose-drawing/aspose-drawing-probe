---
title: Aspose.Drawing next-generation draw image engine for .NET7 and higher
description: Aspose.Drawing program library for image drawing. Alternative replacement to System.Drawing. Image drawing .NET (C#) for graphic application development.
keywords: [image drawing, draw an image]
---

# Aspose.Drawing next-generation draw image engine for .NET7 and higher

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Drawing images with graphic libraries is a very demanding operation for developers, researchers, students and managers who create graphic applications and services on .NET platform. Aspose.Drawing is a modern cross-platform image library with enhanced capabilities. With the Aspose library for .NET it is possible effectively draw lines and shapes using different Pen and Brush objects, create texts with different fonts and styles, make various transformations and raster images in all commonly used graphics file formats. The ready-to-use graphic library helps to increase productivity, dramatically reduce development and time-to-market period. The Microsoft System.Drawing.Common library recently changed its support for non-Windows platforms and Aspose.Drawing will be a proper replacement for drawing images.

</p>

## System.Drawing replacement with Aspose.Drawing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Drawing for .NET is a powerful cross-platform program library for 2D graphics drawing. The Aspose library can be used as an alternative to System.Drawing package.
On May 22, 2023, the Microsoft Learn portal published an article about a breaking change: 
<a href="https://learn.microsoft.com/en-us/dotnet/core/compatibility/core-libraries/6.0/system-drawing-common-windows-only">System.Drawing.Common only supported on Windows</a>. Now, if you try to compile a program with the System.Drawing.Common package on non-Windows environments, the exception will be thrown that your platform is not supported. Despite of you can still switch off this warning, it is recommended to migrate to other libraries. Aspose.Drawing is a good choice for drawing application development for .NET Framework, .NET Core and for Xamarin applications for Windows, Linux, Android, Azure Functions or Blazor WebAssembly.
</p>


## Aspose.Drawing alternative to System.Drawing

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Aspose.Drawing package is available for download from the  <a href="https://www.nuget.org/packages/Aspose.Drawing">NuGet package manager repository</a>. The Aspose package supports any 32-bit or 64-bit operating system where .NET Framework or .NET Core is installed and fully compatible with System.Drawing API. Please find the API description on <a href="https://products.aspose.com/drawing/net/">Aspose .NET APIs for 2D Graphics Drawing</a> product page.
</p>


## Cross platform graphics for C# (.NET)

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Graphic libraries for .NET are used not only on the Windows platform but also very popular for other systems like Linux, Android or WebAssembly. The big advantage of Aspose.Drawing - is a cross-platform solution, you can use it at the same time on different platforms. Development with the same library streamlines the application creation process. You can reuse once-developed code on multiple platforms. Aspose.Drawing library capabilities provides you with a whole range of 2D drawing features as:
</p>

- Creating bitmaps from scratch or loading from files.
- Drawing lines, Bezier curves, splines, and arcs.
- Drawing shapes such as rectangles, polygons, eclipses, etc.
- Processing and drawing graphics paths.
- Rendering text with different fonts and styles.
- Using different pen widths and styles.
- Using solid and texture brushes.
- Alpha blending and anti-aliasing lines and shapes.
- Working with clip regions.
- Using affine transformations.

You can follow a link to the <a href="https://docs.aspose.com/drawing/net/">Aspose.Drawing for .NET documentation</a> for a full feature list.

## Cross platform drawing API for C# (.NET)

### Drawing lines and shapes

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
In this example, we create a series of graphic primitives such as lines, rectangles and ellipses using the <a href="https://reference.aspose.com/imaging/net/aspose.imaging/graphics/drawpath/">DrawPath method</a>. At the beginning, we create a bitmap with a size of 1000x800 pixels and 32 bits per pixel color. Then we define an object Pen with two properties: color `Blue` and width `2` pixels for drawing images, and a <a href="https://reference.aspose.com/imaging/net/aspose.imaging/graphicspath/">Path object</a>. After that, we adding subsequently to the Path 2 lines with start and end X, Y coordinates: from `(100, 100)` to `(1000, 400)` and next line from `(1000, 600)` to `(300, 600)`; a Rectangle with shapes: left upper corner `(0, 0)`, width `200` and height `400` px; and an Ellipse object fitted to a rectangle: left upper corner `(10, 200)` width `450` and height `300` px. Using DrawPath method with described Pen object we draw the Path on the created bitmap. Finally we raster the image and save it into PNG file.
</p>

C# code example:
```cs
using System.Drawing;
using System.Drawing.Drawing2D;

namespace Aspose.Drawing.Examples.CSharp.LinesCurvesShapes
{
    class DrawPath
    {
        public static void Run()
        {
            //ExStart: DrawPath
            Bitmap bitmap = new Bitmap(1000, 800, System.Drawing.Imaging.PixelFormat.Format32bppPArgb);
            Graphics graphics = Graphics.FromImage(bitmap);

            Pen pen = new Pen(Color.FromKnownColor(KnownColor.Blue), 2);
            GraphicsPath path = new GraphicsPath();
            path.AddLine(100, 100, 1000, 400);
            path.AddLine(1000, 600, 300, 600);
            path.AddRectangle(new Rectangle(500, 350, 200, 400));
            path.AddEllipse(10, 250, 450, 300);
            graphics.DrawPath(pen, path);

            bitmap.Save(RunExamples.GetDataDir() + @"LinesCurvesShapes\DrawPath_out.png");
            //ExEnd: DrawPath
        }
    }
}
```

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
The C# code above will draw the following image with Lines, Rectangle and Ellipse:
</p>

<img src="./drawing/DrawPath_out.png" alt="Draw Line Rectangle Ellipse Path " width="1000" height="800"/>

You can find more examples in <a href="https://reference.aspose.com/imaging/net/aspose.imaging/graphics/drawpath/">Aspose documentation</a>.


### Drawing arcs

<p align='justify'>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

{% gist aspose-com-gists/660f3761ba6652f5bbd06bd535ac4bf9 draw-arc.cs %}

<img src="./drawing/DrawArc_out.png" alt="Draw Arc with Aspose.Drawing" width="" height=""/>

<a href="https://github.com/aspose-drawing/Aspose.Drawing-for-.NET">Aspose.Drawing for .NET Examples</a>

</p>
