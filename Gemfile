source "https://rubygems.org"

# For local development we'll use Jekyll 4.4.1
gem "jekyll", "~> 4.4.1", group: :jekyll_plugins

# GitHub Pages - note that we're commenting this out for local development
# When deploying to GitHub Pages, they will use their own version
# gem "github-pages", group: :jekyll_plugins

gem "webrick", "~> 1.9.1"

# Add logger gem to silence warning
gem "logger"

# Jekyll plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17.0"
  gem "jekyll-seo-tag", "~> 2.8"
  # Add sass-embedded to use modern Sass features
  gem "sass-embedded", "~> 1.85.1"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.8.0` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.8.0", :platforms => [:jruby] 