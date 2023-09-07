# Forms

> **The `vh` unit** stands for viewport height, and is relative to 1% of the `height` of the viewport.

## form | method attribute

The `method` attribute specifies how to send form-data to the URL specified in the `action` attribute. The form-data can be sent via a `GET` request as URL parameters (with `method="get"`) or via a `POST` request as data in the request body (with `method="post"`).

## fieldset element

The **`<fieldset>`** [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) element is used to group several controls as well as labels ([``](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label)) within a web form.

~~~~
<form>
  <fieldset>
    <legend>Choose your favorite monster</legend>

    <input type="radio" id="kraken" name="monster" value="K" />
    <label for="kraken">Kraken</label><br />

    <input type="radio" id="sasquatch" name="monster" value="S" />
    <label for="sasquatch">Sasquatch</label><br />

    <input type="radio" id="mothman" name="monster" value="M" />
    <label for="mothman">Mothman</label>
  </fieldset>
</form>

~~~~

> The `rem` unit stands for root `em`, and is relative to the font size of the `html` element.

## input | type attribute

Specifying the `type` attribute of a form element is **important for the browser to know what kind of data it should expect**. If the `type` is not specified, **the browser** will **default** to **`text`**.

## input | type="submit"

The first `input` element with a `type` of `submit` is automatically set to submit its nearest parent `form` element.

## Custom validation

### password - minlength attribute

~~~~
<label for="new-password">Create a New Password: 
	<input id="new-password" type="password" minlength="8" required /></label>
~~~~

### password - pattern attribute

With `type="password"` you can use the `pattern` attribute to define a regular expression that the password must match to be considered valid.

A regular expression which matches eight or more lowercase letters or the digits `0` to `5`:

~~~~
<label for="new-password">Create a New Password: 
	<input id="new-password" type="password" pattern="[a-z0-5]{8,}" required />
</label>
~~~~

## select element

Adding a dropdown to the form is easy with the `select` element. The `select` element is a container for a group of `option` elements, and the `option` element acts as a label for each dropdown option. Both elements require closing tags.

~~~~
<label>How did you hear about us?
	<select>
        <option>(select one)</option>
        <option>freeCodeCamp News</option>
        <option>freeCodeCamp YouTube Channel</option>
        <option>freeCodeCamp Forum</option>
        <option>Other</option>
    </select>
</label>
~~~~
> vw unit?

> **last-of-type**
>
> You can select the last element of a specific type using the `last-of-type` CSS pseudo-class, like this:  
> ~~~~
> p:last-of-type { }
> ~~~~
>
> 
