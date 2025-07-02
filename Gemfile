# frozen_string_literal: true

source "https://rubygems.org"

# gem "rails"

gem "jekyll", "~> 4.4"

# custom
gem "webrick", "~> 1.7"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sitemap"
end

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]