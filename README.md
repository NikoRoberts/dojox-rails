# Dojox with Rails

This gem allows you to use the Dojox library (which is part of the [dojo toolkit](http://dojotoolkit.org/)) with the cool Ruby on Rails framework. See also [dojo-rails](https://github.com/robin850/dojo-rails) and [dijit-rails](https://github.com/robin850/dijit-rails) if you are a Dojo fan.

## Installation and basic use

Just open up your application's `Gemfile` and add the following lines (commonly to your `:assets` group):

```ruby
group :assets do
  # ...
  gem 'dojo-rails'
  gem 'dojox-rails'
end
```

Just run the `bundle` command to install the gems. Then, in your javascript files just use the `require` function and load your Dojox assets just like that (here a gist with CoffeeScript):

```coffeescript
"dojox/charting/Chart",
 
    // Require the theme of our choosing
    "dojox/charting/themes/Claro",
require(["dojox/charting/Chart", "dojox/charting/themes/Claro"], (chart, theme) ->
  # ... Here your code
)
```

## Contributing

### Code

If you want to improve the project or fix something you just have to:

* Fork the project
* Clone the repository on your local machine
* Create a new branch with `git checkout -b new_feature`
* Make changes and commit them
* `git push origin master`
* And finally open a new pull request on this repo

### Bugs and issues

For issues and bugs, please open a [new ticket](https://github.com/robin850/dojox-rails/issues/new) to the issue tracker. Thanks.

## License

This project is released under the MIT license. See the `LICENSE` file for more information.