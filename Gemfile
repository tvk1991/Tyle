source "https://rubygems.org"

# GitHub Pages dependencies
gem "github-pages", group: :jekyll_plugins

# Jekyll
gem "jekyll"

# Theme (minima là theme mặc định của GitHub Pages)
gem "minima"

# Các gem khác nếu cần
group :jekyll_plugins do
  gem "jekyll-sitemap"
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
end

# Các gem cho development (không cần thiết cho GitHub Pages)
group :development do
  gem "jekyll-admin"
end

# Windows không hỗ trợ sassc
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end
