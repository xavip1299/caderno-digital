source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.3.0"

# Tema
gem "minima", "~> 2.5"

# Plugins Jekyll essenciais
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
  gem "jekyll-paginate"
  gem "jekyll-gist"
  gem "jekyll-include-cache"
end

# GitHub Pages compatibility  
gem "github-pages", group: :jekyll_plugins

# Performance watcher para desenvolvimento
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Timezone
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end