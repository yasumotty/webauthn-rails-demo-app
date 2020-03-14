# frozen_string_literal: true

source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby File.read(".ruby-version").strip

gem 'rails', "~> 6.0.0"
gem "webauthn", "~> 2.2.0"

gem 'bootsnap', '~> 1.4', require: false
gem 'pg', '~> 1.1'
gem 'puma', '~> 4.2'
gem "rollbar", "~> 2.16"
gem 'sassc-rails', '~> 2.0'
gem 'webpacker', '~> 4.0'

group :production do
  gem "rack-host-redirect", "~> 1.3"
end

group :development, :test do
  gem 'byebug', '~> 11.0', platforms: [:mri, :mingw, :x64_mingw]
  gem "dotenv-rails", '~> 2.7'
  gem 'rubocop', '~> 0.73.0', require: false
  # rubocop-rails 2.2 => 2.3 broke the build - adopt more conservative gem constraint
  gem 'rubocop-rails', '~> 2.2.1', require: false
end

group :development do
  gem 'listen', '~> 3.1'
  gem 'spring', '~> 2.1'
  gem 'spring-watcher-listen', '~> 2.0'
  gem 'web-console', '~> 4.0'
end

group :test do
  gem 'capybara', '~> 3.26'
  gem 'minitest-stub_any_instance', '~> 1.0'
  gem 'selenium-webdriver', '~> 3.142'
  gem 'webdrivers', '~> 4.1'
end
