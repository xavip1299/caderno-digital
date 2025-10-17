source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.3.0"

# Tema padrão
gem "minima", "~> 2.5"

# Plugins essenciais para GitHub Pages
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
  gem "jekyll-paginate"
end

# Compatibilidade com Windows
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance no Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Para compatibilidade com GitHub Pages
gem "github-pages", group: :jekyll_plugins