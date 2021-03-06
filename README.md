# Revelar

Create stunning presentations in **Markdown** using [Reveal.js](https://github.com/hakimel/reveal.js) from the confort of your command line.

## Creating a new presentation

Start by installing the `revelar` utility globally:

```shell
npm install --g revelar
```

Create a new presentation project.

```shell
revelar create presentation-name
```

This will create a new folder called `presentation-name` with:

* A `slides` folder to contain your slides divided into multiple sections;
* A `themes` folder to contain custom themes (like a sample `yellow.css`);
* And the `revelar_config.json` with configuration parameters.

## Running the server

Once the project is created, start the server to see the slides:

```shell
revelar
```

And point your browser to [http://0.0.0.0:8000/](http://0.0.0.0:8000/).

## Anatomy of a slide

Inside the `slides` folder you can place as many Markdown files as you want.

Each file will correspond to a different section in your presentation.

Each section can contain multiple slides, each separated by a `--`.

Here is an example of a section writen in a Markdown file:

```markdown
# Revelar
## This is awesome

[paulo.ragonha.me](http://paulo.ragonha.me)

[@pirelenito](http://twitter.com/pirelenito)

--
# A second slide

--
# And a third
```

## Themes

It is possible to change the theme of your presentation from the [available Reveal.js themes](https://github.com/hakimel/reveal.js#theming) by specifying it in the `revelar_config.json` file:

```json
{
  "theme": "sky"
}
```

### Custom themes

You can place your custom theme files inside the `themes` folder and use them the same way as a default theme.

## Acknowledgments

This is build on top of the amazing [Reveal.js](https://github.com/hakimel/reveal.js) framework.

## Author

[Paulo Ragonha](http://paulo.ragonha.me).
