# template-html

[![NPM Version](https://img.shields.io/npm/v/template-html.svg)](https://www.npmjs.com/package/template-html)
[![Build Status](https://img.shields.io/travis/grit96/template-html.svg)](https://travis-ci.org/grit96/template-html)
[![Dependency Status](https://img.shields.io/david/grit96/template-html.svg)](https://david-dm.org/grit96/template-html)

Generate static HTML files from templates and content files. [gulp-template-html](https://github.com/grit96/gulp-template-html) is a Gulp plugin for this with example usage.


## Installation
```sh
$ npm install -g template-html
```

## Help

```
Usage: template-html content.html -t template.html [options]

-h|--help      display this help message
-v|--version   display the version number
-o|--output    directory to output processed HTML
-t|--template  template file to use
--tag          keyword to use be used in HTML placeholder define and build comments
--build-tag    keyword to use be used in HTML placeholder build comments (overrides --tag)
--define-tag   keyword to use be used in HTML placeholder define comments (overrides --tag)
```

## Documentation

### `Templator(options)`
Creates a new `Templator` instance.

#### Params
- **Object** `options`: An object containing the following fields:
 - `templateFile` (String): Path to template file to use.
 - `tag` (String): Keyword to use be used in HTML placeholder comments.

### `processFile(contentFile)`
Run the contents of an HTML file through the `Templator`

#### Params
- **String** `contentFile`: Path to HTML file to be processed

#### Return
- **String** The processed HTML

### `processContent(content)`
Generate HTML from template file and content file

#### Params
- **String** `content`: HTML content to be used in template

#### Return
- **String** The processed HTML


## How to contribute

1. File an issue in the repository, using the bug tracker, describing the
   contribution you'd like to make. This will help us to get you started on the
   right foot.
2. Fork the project in your account and create a new branch:
   `your-great-feature`.
3. Commit your changes in that branch.
4. Open a pull request, and reference the initial issue in the pull request
   message.


## License
See the [LICENSE](./LICENSE) file.
