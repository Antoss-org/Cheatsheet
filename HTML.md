## Text

- <h1></h1>
- <h2></h2>
- <h3></h3>
- <h4></h4>
- <h5></h5>
- <h6></h6>

- <p></p>
- <!-- -->

- <ul></ul>
- <ol></ol>
- <li></li>

- <em></em>
- <strong></strong>


## Semantic

- <main></main>
- <footer></footer>
- <section></section>


## Links

- <a href="" target="{_blank}"></a>

<figure>
	<img src="" alt="">
	<figcaption></figcaption>
</figure>


## Interactive

- <button type="{submit}"></button>

<form action="">
	<fieldset>
		<legend></legend>
			<input type="{text||**radio||checkbox**}" name="*[1]" value="*[2]" id="" checked required>
			<label for="*[3]"></label>
			<input type="{**text**||radio||checkbox}" name="" placeholder="" id="" required>
	</fieldset>
</form>
*[1] With multiple inputs like radio or checklist, name has to be the same so they relate to each other, and *[2], add different values for each choice
*[3] If you want to put the label as its own element instead of nesting input inside label, you have to put the for attribute, with its content having the same name as the id of the input


## Metadata

- <!DOCTYPE html>
- <html lang="{en}"></html>
- <head></head>
- <body></body>

### Inside head

- <title></title>
- <meta charset="{UTF-8}">