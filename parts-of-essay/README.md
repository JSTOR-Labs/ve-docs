# The Parts of an Essay

While not all essays written for print are the same, they usually share similar parts:

* A Title
* An Author
* A description or abstract
* Sections
* Paragraphs
* Footnotes/Endnotes/References

All of these parts can be found in visual essays, but there are also additional elements:

* Images and Image Galleries
* Maps and Layers
* References that Connect to Linked Open Data
* Network Graphs

To make these new features possible, a visual essay relies on some level of coding that describes for readers what should appear on the screen at any given time. Our goal in creating the Visual Essay Tool has been to balance the performative possibilities of your essay with the complexity of code. In doing so, we have sought to make the technical hurdle of writing code as accessible as possible, preferring to hide messy details that are likely to be unproductive for authors and expose layers that could prove helpful for making visual arguments.

The structure of a visual essay is similar to a traditional printed essay with some key differences. First, it begins with a basic configuration tag that specifies the nature of the page/essay for the reader.

# The Configuration Tag

The `param ve-config` tag is not technically required for an essay to render, but it supplies some crucial information that any serious essay is likely to include. The form of the configuration tag is:

`<param ve-config
    attribute1="value for this attribute"
    attribute2="value for this attribute"
    ...
    finalattribute="value for this attribute">`

Note that the tag begins with a left caret (<) and ends with a right caret after the final attribute (>). 

![An example configuration tag](config-tag.png)

The value for a given attribute is always enclosed in double quotations marks ("). In this example we can see the following *attributes* are defined for this essay:

|Attribute|Description of the value|
|---|---|
|title|The title of your essay|
|banner|The URL of the image that will appear in your banner. Ideally, this image is very wide but not very tall.|
|layout|Specify a vertical essay with `vtl`|
|num-maps|The number of maps in your essay.|
|num-images|The number of images in your essay.|
|num-primary-sources|The number of primary sources in your essay.|
|author|That's probably you!|
