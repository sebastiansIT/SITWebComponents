# SelectImageElement
The SelectImageElement class represents a [&lt;sit-select-image&gt; Element](./CustomElement.md).
These elements also share all of the properties and methods of other HTML elements
via the [HTMLElement](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement)
interface.

It is the Javascript representation of the web component [select-image](../README.md).

## Properties
This class inherits the properties of [HTMLElement](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement),
and of [Element](https://developer.mozilla.org/en-US/docs/Web/API/Element) and
[Node](https://developer.mozilla.org/en-US/docs/Web/API/Node).

<dl>
  <dt><code>SelectImageElement.defaultValue</code> <span class="readonly">Read only</span></dt>
  <dd><p>This property gives you access to the initial value of the element.</p></dd>

  <dt><code>SelectImageElement.value</code></dt>
  <dd><p>The actual selected image as an Base64 encoded data URL. If no image
  is selected the value is the default value.</p></dd>
</dl>

## Methods
<dl>
  <dt><code>SelectImageElement.clear</code></dt>
  <dd><p>Removes the image and set the value to undefined.</p></dd>
  <dt><code>SelectImageElement.revert</code></dt>
  <dd><p>Revert the selected image and revert to the default image.</p></dd>
  <dt><code>SelectImageElement.select</code></dt>
  <dd><p>Opens a file selection dialog to select a new image.</p>
  <p>This function can only be called in reaction to a user triggerd event.</p></dd>

## Events
Listen to these events using addEventListener().
<dl>
  <dt>change</dt>
  <dd>Fires when the value of an <sit-select-image> element has been changed. The Event has one Property detail.value containing the actual value.</dd>
</dl>
