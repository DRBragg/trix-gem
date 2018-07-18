# Trix Gem

Want to include Basecamp's awesome [Trix WYSIWYG
editor](http://trix-editor.org) in your Ruby on Rails application?
You've come to the right place!

## Installation

The `trix-gem` makes it easy to drop Trix into Rails with the asset pipeline.

Add this line to your application's Gemfile:

```ruby
gem 'trix-gem'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install trix-gem

## Usage

Import Trix styles in `app/assets/stylesheets/application.css`:

```css
*= require trix
```

Require Trix Javascript magic in `app/assets/javascripts/application.js`:

```js
//= require trix
```

Finally, any place where you would like to use the Trix editor in your
forms, just use the `trix_editor` helper:

```ruby
f.trix_editor :body
```

If you are using the [Formtastic](https://github.com/justinfrench/formtastic) gem or the [Simple Form](https://github.com/plataformatec/simple_form) gem, you can do this:

```ruby
f.input :body, as: :trix_editor
```

## Trix

For the official Trix Github repository, go
[here](https://github.com/basecamp/trix).

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/DRBragg/trix-gem. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Trix-gem project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/DRBragg/trix-gem/blob/master/CODE_OF_CONDUCT.md).
