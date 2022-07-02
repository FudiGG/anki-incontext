# InContext

An [Anki](https://apps.ankiweb.net/) add-on that works as a template filter to show random example sentences for vocabulary each time a card is viewed.

You just have to put a filter like this in your [card template](https://docs.ankiweb.net/templates/intro.html):

```
{{incontext:Front}}
```

Here the add-on will show a random English example sentence containing the word in the `Front` field.

You can specify the language using the `lang` option:

```
{{incontext lang=en:Front}}
```

Currently supported values are `en` (English) and `tr` (Turkish). `en` is the default.

Currently, English example sentences are fetched from the [Oxford English Dictionaries](https://www.lexico.com/) and the [Oxford Learner's Dictionaries](https://www.oxfordlearnersdictionaries.com/).
Turkish sentences are fetched from https://sozluk.gov.tr/

More sites and languages may be supported in the future.

Fetched sentences are saved locally in the `user_files/sentences.db` file and used in subsequent reviews of the same card.

The add-on has an experimental graphical interface to manage sentences that can be accessed from **Tools > InContext**.

Download this deck for a demo of the add-on: https://drive.google.com/file/d/1Era5ksSa59xjB3ZbVQsdoTbQEigzh6Bi/view?usp=sharing

## TODO
- [ ] Improve interface.
- [ ] Support more languages and fetchers.
