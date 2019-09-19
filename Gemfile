source 'https://rubygems.org'

branch = ENV.fetch('SOLIDUS_BRANCH', 'master')
gem 'solidus', github: 'solidusio/solidus', branch: branch

gem 'solidus_auth_devise'

# Needed to help Bundler figure out how to resolve dependencies, otherwise it takes forever to
# resolve them
if branch == 'master' || Gem::Version.new(branch[1..-1]) >= Gem::Version.new('2.10.0')
  gem 'rails', '~> 6.0'
else
  gem 'rails', '~> 5.0'
end

gemspec
