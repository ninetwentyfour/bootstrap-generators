# Bootstrap Generators

Bootstrap-generators provides Twitter Bootstrap generators for Rails 3.1. Bootstrap is a toolkit from Twitter designed to kickstart development of webapps and sites. Checkout http://twitter.github.com/bootstrap.

## Rails 3.1 setup

This gem requires the use of rails 3.1.

### Installation

In your Gemfile, add this line:

  `gem 'bootstrap-generators'`

By default Bootstrap Generators requires SimpleForm. Add the dependency on your Gemfile:

  `gem 'simple_form', '~> 1.5'`

If you don't want to use SimpleForm, and instead use the default Rails form builder, just call the install generator with `--form_builder=form_builder`.

Then run the following commands:

  `bundle install`
  `rails generate bootstrap:install`

Once you've done that, any time you generate a controller or scaffold, you'll get [Bootstrap](http://twitter.github.com/bootstrap/) templates.

## Form builders

### Default Rails form builder

  `rails generate bootstrap:install --form_builder=form_builder`

### SimpleForm

  `rails generate bootstrap:install --form_builder=simple_form`

## Layouts

There are three layouts available, based on the quick-start examples:

* hero (default; based on [this template](http://twitter.github.com/bootstrap/examples/hero.html))
* fluid (based on [this template](http://twitter.github.com/bootstrap/examples/fluid.html))
* container-app (based on [this template](http://twitter.github.com/bootstrap/examples/container-app.html))

To select one of these layouts just pass the option '--layout=LAYOUT' to the install generator.

