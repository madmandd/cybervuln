# frozen_string_literal: true

source "https://rubygems.org"
gemspec
gem "jekyll", "~> 4.3.2"

group :jekyll_plugins do
    gem 'rubygems-update', '~> 3.4', '>= 3.4.22'
    gem "jekyll-feed", "~> 0.12"
    gem "jekyll-seo-tag"
    gem 'rspec-core'
    gem "jekyll-notion", "~> 2.4.1"
    gem 'jekyll-content-security-policy-generator'
end
gem 'sass-embedded', '~> 1.69', '>= 1.69.5'

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
    gem "tzinfo", ">= 1", "< 3"
    gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]

gem "webrick", "~> 1.8"
