# Crisp-Components

This is a library that provides a collection of UI themes for WPF applications developed using .NET Core 7. Designed to provide a modern and crisp look and feel across all controls in your application. The themes are implemented using XAML styles and templates.

## Features
Predefined themes for common UI elements, such as buttons, text boxes, and list boxes.
Easy-to-use XAML styles and templates that can be applied to any WPF control.
Supports light and dark themes.
Fully customizable to fit the needs of your application.

## Installation
To install Crisp.Components, simply download the source code and include the Crisp.Components.dll file in your project references.

Alternatively, you can also use NuGet to install the package by running the following command in the Package Manager Console:

```powershell
Install-Package Crisp.Components
```

## Usage
Once you have included the Crisp.Components library in your project, you can easily apply the themes to your WPF controls by referencing the appropriate dictionary in your XAML.

Here's an example of how to use the ControlsDictionary.xaml in your application:

```xml
<Application.Resources>
    <ResourceDictionary>
        <ResourceDictionary.MergedDictionaries>
            <ResourceDictionary Source="/Crisp.Components;component/Themes/MergedDictionary.xaml"/>
        </ResourceDictionary.MergedDictionaries>
    </ResourceDictionary>
</Application.Resources>
```

Similarly, you can reference the other dictionaries provided by the library by replacing the Source attribute with the appropriate dictionary file name.

## Customization
The themes provided by Crisp.Components are fully customizable. You can modify the styles and templates provided by the library to match your application's branding and design.

To customize the themes, you can create a new XAML file that merges the desired dictionary and overrides the styles and templates defined in it.

For example, to customize the ControlDictionary.xaml, you can create a new XAML file and add the following code:

```xml
<ResourceDictionary.MergedDictionaries>
    <ResourceDictionary Source="/Crisp.Components;component/Themes/MergedDictionary.xaml"/>
</ResourceDictionary.MergedDictionaries>

<!-- Override the default style for the Button control -->
<Style TargetType="{x:Type Button}">
    <Setter Property="Background" Value="Red"/>
</Style>
```

In this example, we're overriding the default style for the Button control and setting its background color to Red.

## Contributing
Contributions to this library are welcome! If you find a bug or have a feature request, please open an issue on GitHub. If you would like to contribute code, please fork the repository and submit a pull request with your changes.

## License
This library is released under the MIT License. See the LICENSE file for details.
