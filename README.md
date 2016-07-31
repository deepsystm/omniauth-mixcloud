# OmniAuth MixCloud

This gem contains the MixcloudCloud strategy for OmniAuth 1.0.

## Installing

Add to your `Gemfile`:

```ruby
gem 'omniauth-mixcloud', github: 'deepsystm/omniauth-mixcloud'
```

Then `bundle install`.

## Basic Usage

    use OmniAuth::Builder do
    	provider "mixcloud", ENV['MIXCLOUD_CLIENT_ID'], ENV['MIXCLOUD_SECRET']
    end
    
Add to `config/initializers/devise.rb` to use with Devise

    config.omniauth :mixcloud, 
        Rails.application.secrets.mixcloud_id, 
        Rails.application.secrets.mixcloud_secret

## Supported Flows

Supports the Server-side Flow as described in the the [MixCloud docs](http://www.mixcloud.com/developers/#authorization).

Copyright (c) 2011 by Rich Morgan and MixCloud

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
