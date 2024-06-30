source "https://rubygems.org"

gem "jekyll", "~> 4.3.3"
gem "minima", "~> 2.5"
gem "minimal-mistakes-jekyll"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]

# (A) THE BELOW HAS TO BE ADDED FOR ONLINE RUNNING - REMOVE FOR LOCAL RUNNING
# source "https://rubygems.org"
# gem "github-pages", group: :jekyll_plugins
# gem "jekyll-include-cache", group: :jekyll_plugins