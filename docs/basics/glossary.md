# Glossary


<a name="addon"></a>
### Addon

    Modules, Field Types, Plugins, Themes, and Extensions.

A bundle of organized code that you can use to add functionality to your application.


<a name="builder"></a>
### Builder

	<?php namespace Anomaly\ExampleModule\Example\Table;

	use Anomaly\Streams\Platform\Ui\Table\TableBuilder;

	class ExampleTableBuilder extends TableBuilder
	{
		// Definitions
	}

A class that holds and/or provides the [definitions](#definition) for various [components](#component) used to build larger objects like [forms](#form) and [tables](#table). The builder class is the primary type of class a developer will use when building the addons for their application.


<a name="component"></a>
### Component

An object that helps build larger objects like [forms](#form) and [tables](#table). Form actions, form fields, table row buttons, table columns, and table filters are just some examples of components.


<a name="definition"></a>
### Definition

**Shortest Example**

	['edit']

**Full Example**

	[
		'type' => 'warning',
		'text' => 'Edit',
		'icon' => 'pencil',
		'href' => 'admin/example/edit/{entry.id}'
	]

An array representation of a [component](#component) that is normalized, processed and converted into the [component's](#component) class. Definitions are usually used with [builders](#builder).