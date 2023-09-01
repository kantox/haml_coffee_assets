source 'https://rubygems.org'

gemspec

gem "rails", "~> #{ENV['RAILS_VER'] || raise("missing rails version")}"
gem "sprockets", "~> #{ENV['SPROCKETS_VER'] || raise("missing sprockets version")}"

#
# The gem is bugged/incompatible in later versions due to nokogiri conflict
# and ruby versions
#   uninitialized constant Nokogiri::HTML4
#
if ENV['RUBY_VERSION'].to_f <= 2.4
  gem "loofah", "~> 2.20.0"
end

