---
title: Getting Started
page_title: Getting Started
description: Getting Started
slug: radtoolbar-getting-started
tags: overview
published: True
position: 2
---

# Getting Started

This tutorial will walk you through the creation of a sample application that contains __RadToolBar__. 

* [Assembly References](#assembly-references)
* [Add RadToolBar to the Project](#add-radtoolbar-to-the-project)
* [Populating with Data](#populating-with-data)

## Assembly References

In order to use the __RadToolBar__ control in your projects, you have to add references to the following assemblies:			

* __Telerik.Windows.Controls__
* __Telerik.Windows.Controls.Navigation__

## Add RadToolBar to the Project

Before proceeding with adding __RadToolBar__ to your project, make sure the required assembly references are added to the project. 

You can add __RadToolBar__ manually by writing the XAML code in __Example 1__. You can also add the control by dragging it from the Visual Studio Toolbox and dropping it over the XAML view.

#### __[XAML] Example 1: Adding RadToolBar in XAML__

{{region xaml-radtoolbar-getting-started_0}}
	<telerik:RadToolBar />
{{endregion}}


>In order to use __RadToolBar__ in XAML you have to add the namespace declaration shown in __Example 2__:
>#### __[XAML] Example 2: Declaring Telerik Namespace__
>{{region telerik-schemas}}
>    xmlns:telerik="http://schemas.telerik.com/2008/xaml/presentation"
>{{endregion}}

If you run the application you will see an empty toolbar as demonstrated in __Figure 1__. 

#### __Figure 1: The empty toolbar generated by the code in Example 1__

![Empty RadToolBar](images/empty-toolbar.png)

## Populating with Data

In order to populate the __RadToolBar__ control with data in XAML, you can add a few __RadButtons__ to it and set their Content property as in __Example 3__.

#### __[XAML] Example 3: Adding RadButtons in XAML__

{{region xaml-radtoolbar-getting-started_1}}
	<telerik:RadToolBar>
		<telerik:RadButton Content="FILE" />
		<telerik:RadButton Content="EDIT " />
		<telerik:RadButton Content="VIEW" />
		<telerik:RadButton Content="BUILD" />
		<telerik:RadButton Content="DEBUG" />
		<telerik:RadButton Content="HELP" />
	</telerik:RadToolBar>
{{endregion}}

Running the application will result in a populated __RadToolBar__ as shown in __Figure 2__.

#### __Figure 2: RadToolBar with static items__

![Populated RadToolBar](images/populated-toolbox.png)

Adding static items in XAML is good for scenarios when you know in advance the contents toolbox. However, in most cases, you have to bind your RadToolBar to a collection of objects. You can achieve this through the **ItemsSource** property of the control.

>You can have a look at [the following blog post](http://www.telerik.com/blogs/how-to-databind-telerik-s-toolbar) for a good example of how to bind the control.

## See Also

 * [ToolBarTray Overview]({%slug radtoolbartray-overview%})

 * [Item Alignment]({%slug radtoolbar-features-itemalignment%})

 * [RadToolBar API Reference](https://docs.telerik.com/devtools/wpf/api/telerik.windows.controls.radtoolbar)