source "https://rubygems.org"

# Match GitHub Pages' supported Jekyll and plugin versions without pulling in
# its full deployment bundle, which keeps local builds lightweight.
gem "jekyll", "~> 3.10.0"
# Ruby 4 no longer bundles this standard library, while Jekyll 3 still uses it.
gem "base64", "~> 0.3"
gem "bigdecimal", "~> 4.0"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
  gem "jekyll-seo-tag", "~> 2.8.0"
  gem "jekyll-sitemap", "~> 1.4"
  gem "kramdown-parser-gfm", "~> 1.1"
end
