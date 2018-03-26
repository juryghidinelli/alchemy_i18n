# AlchemyCMS Translation Files

Translations files for AlchemyCMS 4.1 and above.

## Usage

The recommended way of adding Alchemy translations is to [download the translation files](https://github.com/AlchemyCMS/alchemy_i18n/tree/master/config/locales) you need
and save them into your apps `config/locales` folder.

Alternatively you could add this gem into your apps `Gemfile`, but then you will add all supported translations into the `I18n.load_path`
which will raise the consumed runtime memory and increase the app start up time.

### Rails translations

This gem only provides translations for Alchemy itself. If you also need translations for ActiveSupport features (like `to_sentence` or `number_with_currency`, etc.)
you should [download the Rails translation files](https://github.com/svenfuchs/rails-i18n/tree/master/rails/locale) and save them into your apps `config/locales` folder.

Alternatively you could add the `rails-i18n` gem into your apps `Gemfile`, but then you will add all supported translations into the `I18n.load_path`
which will raise the consumed runtime memory and increase the app start up time.

### Russian translations

If you want to use Russian translation and have better i18n support, you should put:

```ruby
gem 'russian', '~> 0.6.0'
```

or a gem with similar functionality into your apps `Gemfile`.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).