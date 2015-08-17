source 'https://rubygems.org'

gem 'rails', '4.2.3'
gem 'rails-i18n', :git => "https://github.com/alphagov/rails-i18n.git", :branch => "welsh_updates"
gem 'unicorn', '4.6.3'
gem 'gelf'

gem 'plek', '1.7.0'
gem 'statsd-ruby', '1.0.0', :require => 'statsd'
gem 'htmlentities', '4.3.1'
gem 'shared_mustache', '1.0.0'

if ENV['SLIMMER_DEV']
  gem 'slimmer', :path => '../slimmer'
else
  gem 'slimmer', '8.4.0'
end

if ENV['CDN_DEV']
  gem 'cdn_helpers', :path => '../cdn_helpers'
else
  gem 'cdn_helpers', '0.9'
end

if ENV['API_DEV']
  gem 'gds-api-adapters', :path => '../gds-api-adapters'
else
  gem 'gds-api-adapters', '20.1.1'
end

gem "addressable"
gem 'logstasher', '0.4.8'
gem 'airbrake', '3.1.15'
gem 'invalid_utf8_rejector', '0.0.1'
gem 'rack_strip_client_ip', '0.0.1'

# Note that govuk_frontend_toolkit is only used here for SASS mixins and
# variables. Analytics and other javascript features are provided by static.
gem 'govuk_frontend_toolkit', '~> 4.1.0'
gem 'sass', '3.4.9'
gem 'sass-rails' # required by bootstrap-sass, but not listed as a dependency of it
gem "therubyracer", "0.12.2"
gem 'uglifier'

group :test do
  gem "mocha"
  gem "webmock", :require => false
  gem 'simplecov'
  gem 'simplecov-rcov'
  gem 'ci_reporter'
  gem 'capybara', '2.1.0'
  gem 'poltergeist', '1.3.0'
  gem "launchy"
  gem "shoulda"
  gem "timecop", "0.6.3"
end
