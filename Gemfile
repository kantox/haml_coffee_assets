source 'https://rubygems.org'

gemspec

gem "rack", "~> 2" # Rack 3 is not compatible with Jasmine and fails -- jasmine-3.99.0/lib/jasmine/server.rb:12:in `start': uninitialized constant Rack::Server (NameError)
# json 3.x dropped the `quirks_mode:` keyword that ActiveSupport's JSON
# encoder still passes on Rails < 8.1, raising ArgumentError: unknown
# keyword: quirks_mode. Pin below the breaking major until Rails drops it.
gem "json", "< 3"
gem "rails", "~> #{ENV['RAILS_VER'] || raise("missing rails version")}.0"
gem "sprockets", "~> #{ENV['SPROCKETS_VER'] || raise("missing sprockets version")}"
