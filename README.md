# Getting Started with Xamarin SignaturePad (SfSignaturePad)

This section explains the steps required to configure the Signature Pad.

# Adding SfSignaturePad reference

You can add the Signature Pad reference using one of the following methods:

## Method 1: Adding SfSignaturePad reference from nuget.org

Syncfusion Xamarin components are available in nuget.org. To add Signature Pad to your project, open the NuGet package manager in Visual Studio, search for Syncfusion.Xamarin.SfSignaturePad, and then install it.

## Method 2: Adding SfSignaturePad reference from toolbox

Syncfusion also provides Xamarin Toolbox. Using this toolbox, you can drag the SfSignaturePad control to the XAML page. It will automatically install the required NuGet packages and add the namespace to the page. To install Syncfusion Xamarin Toolbox, refer to this Toolbox.

## Method 3: Adding SfSignaturePad assemblies manually from the installed location

If you prefer to manually reference the assemblies instead of referencing from NuGet, add the following assemblies in respective projects.

# Adding a namespace
Add the following namespace.

**[XAML]**

```
xmlns:signature="clr-namespace:Syncfusion.XForms.SignaturePad;assembly=Syncfusion.SfSignaturePad.XForms"
```
**[C#]**

```
using Syncfusion.XForms.SignaturePad;
```
# Creating an SfSignaturePad control
Create an instance for the Signature Pad control, and add it as content.

**[XAML]**

```
<signature:SfSignaturePad>        
</signature:SfSignaturePad>
```

**[C#]**

```
SfSignaturePad signature = new SfSignaturePad();
Content = signature;
```
# Getting Started with a Signature Pad control

The Signature Pad control is configured entirely in C# code or in XAML markup. The following steps explain how to create a Signature Pad and configure their elements.

**[XAML]**
```
<ContentPage xmlns:signature="clr-namespace:Syncfusion.XForms.SignaturePad;assembly=Syncfusion.SfSignaturePad.XForms">
    <StackLayout>
        <Label Text="Input Your Signature"/>
        <Frame>
            <signature:SfSignaturePad HeightRequest="250"/>
        </Frame>
    </StackLayout>
</ContentPage>
```
**[C#]**
```
public MainPage()
{
    InitializeComponent();
    StackLayout stack = new StackLayout();
    Label text = new Label() { Text = "Input Your Signature" };
    Frame frame = new Frame();
    SfSignaturePad signature = new SfSignaturePad();
    signature.HeightRequest = 250;
    frame.Content = signature;
    stack.Children.Add(text);
    stack.Children.Add(frame);
    this.Content = stack;                    
}     
```
## How to run this application?

To run this application, you need to first clone the xamarin-sfsignaturepad-samples repository and then open it in Visual Studio 2022. Now, simply build and run your project to view the output.

## <a name="troubleshooting"></a>Troubleshooting ##
### Path too long exception
If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

## License

Syncfusion has no liability for any damage or consequence that may arise by using or viewing the samples. The samples are for demonstrative purposes, and if you choose to use or access the samples, you agree to not hold Syncfusion liable, in any form, for any damage that is related to use, for accessing, or viewing the samples. By accessing, viewing, or seeing the samples, you acknowledge and agree Syncfusion’s samples will not allow you seek injunctive relief in any form for any claim related to the sample. If you do not agree to this, do not view, access, utilize, or otherwise do anything with Syncfusion’s samples.