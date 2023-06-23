source "https://rubygems.org"

# Not needed for gh pages (already a dependency of github-pages)
# gem "jekyll", "~> 4.3.2"

# This is needed to run jekyll locally using the docker image
gem "webrick"

gem "github-pages", "~> 228", group: :jekyll_plugins

# PLUGINS
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.15.1"
  gem 'jekyll-seo-tag', '~> 2.8'
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
