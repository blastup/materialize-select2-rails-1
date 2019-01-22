# Select2 for Rails asset pipeline modified for Materialize framework

[Select2](https://github.com/select2/select2) is a jQuery based replacement for select boxes. It supports searching, remote data sets, and infinite scrolling of results.

`materialize-sass` is a Sass powered version of [Materialize](http://materializecss.com), a modern responsive front-end framework based on Material Design.

The `materialize-select2-rails` gem integrates the `Select2` jQuery plugin with the Rails asset pipeline modified for materialize-sass.

## Usage

### Install materialize-select2-rails gem

Add `materialize-select2-rails` to your Gemfile and run `bundle install`:

  gem "materialize-select2-rails"

### Include materialize-select2-rails javascript assets

Add the following to your `app/assets/javascripts/application.js`:

  //= require materialize-select2

To add `materialize-select2-full.js` instead of `materialize-select2.js`, add the following instead :

  //= require materialize-select2-full

### Include materialize-select2-rails stylesheet assets

Add to your `app/assets/stylesheets/application.css`:

  *= require materialize-select2

Apply the modified theme, by telling Select2 to do so using `materialize` to the [`theme`](https://select2.github.io/examples.html#themes) option when initializing Select2:

    $( "#dropdown" ).select2({
        theme: "materialize"
    });

## Internationalization (i18n)

The languages provided by
[Select2](https://github.com/select2/select2/tree/develop/src/js/select2/i18n) were also included to the `materialize-select2-rails` gem.

af, ar, az, bg, bn, bs, ca, cs, da, de, dsb, el, en, es, et, eu, fa, fi, fr, gl, he, hi, hr, hsb, hu, hy, id, is, it, ja, ka, km, ko, lt, lv, mk, ms, nb, nl, pl, ps, pt, pt-BR, ro, ru, sk, sl, sq, sr, sr-Cyrl, sv, th, tr, uk, vi, zh-CN, zh-TW

## License

Materialize-Selec2-Rails is released under the [MIT License](http://www.opensource.org/licenses/MIT).