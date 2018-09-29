# youtube-dl.rb

Ruby wrapper for [youtube-dl](http://rg3.github.io/youtube-dl/).

[![Build Status](https://travis-ci.org/layer8x/youtube-dl.rb.svg?branch=master)](https://travis-ci.org/layer8x/youtube-dl.rb)
[![Code Climate](https://codeclimate.com/github/layer8x/youtube-dl.rb/badges/gpa.svg)](https://codeclimate.com/github/layer8x/youtube-dl.rb)
[![Test Coverage](https://codeclimate.com/github/layer8x/youtube-dl.rb/badges/coverage.svg)](https://codeclimate.com/github/layer8x/youtube-dl.rb/coverage)
[![Stories in Ready](https://badge.waffle.io/layer8x/youtube-dl.rb.svg?label=ready&title=Ready)](http://waffle.io/layer8x/youtube-dl.rb)

## Install the gem

Add this line to your application's Gemfile:

```ruby
gem 'youtube-dl.rb'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install youtube-dl.rb

## Install youtube-dl
This gem ships with the latest (working) version of youtube-dl built-in, so you don't have to install youtube-dl at all! Unless you want to.

## Usage

Pretty simple.

```ruby
YoutubeDL.download "https://www.youtube.com/watch?v=gvdf5n-zI14", output: 'some_file.mp4'
```

All options available to youtube-dl can be passed to the options hash

```ruby
options = {
  username: 'someone',
  password: 'password1',
  rate_limit: '50K',
  format: :worst
}

YoutubeDL.download "https://www.youtube.com/watch?v=gvdf5n-zI14", options
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Pass test suite (`rake test`)
5. Push to the branch (`git push origin my-new-feature`)
6. Create a new Pull Request

Remember: commit now, commit often.
