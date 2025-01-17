source 'https://rubygems.org'

gemspec

gem 'rake'
gem 'minitest', '~> 5.0'

group :development do
  gem 'yard', '~> 0.9.0'
  gem 'ronn', '~> 0.7.3'
end

group :primary do
  gem 'builder'
  gem 'haml', '>= 4'
  gem 'erubi'
  gem 'markaby'

  case ENV['SASS_IMPLEMENTATION']
  when 'sass'
    gem 'sass'
  when 'sassc'
    gem 'sassc'
  else
    gem 'sass-embedded'
  end

  gem 'coffee-script'
  gem 'livescript'
  gem 'babel-transpiler'
  gem 'typescript-node'
end

platform :mri do
  gem 'duktape', '~> 1.3.0.6'
end

group :secondary do
  gem 'creole'
  gem 'erubis'
  gem 'kramdown'
  gem 'rdoc'
  gem 'radius'
  gem 'asciidoctor', '>= 0.1.0'
  gem 'liquid'
  gem 'maruku'
  gem 'pandoc-ruby'
  gem 'prawn', '>= 2.0.0'
  gem 'pdf-reader'
  gem 'nokogiri'

  if RUBY_VERSION >= '3.1'
    # Was default library, now bundled gem.
    # Needed by prawn tests.
    gem 'matrix'
  end

  platform :ruby do
    gem 'wikicloth'
    gem 'rinku' # dependency for wikicloth for handling links

    gem 'yajl-ruby'
    gem 'redcarpet'
    gem 'rdiscount', '>= 2.1.6'
    gem 'RedCloth'
    gem 'commonmarker'
  end
end
