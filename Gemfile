# frozen_string_literal: true

source "https://rubygems.org"

ruby "3.0.3"

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

# GENERAL #
gem "amazing_print", "~> 1.3"
gem "bootsnap", "~> 1.7", ">= 1.7.3", require: false
gem "cssbundling-rails", "~> 1.1", ">= 1.1.1"
gem "image_processing", "~> 1.12", ">= 1.12.1"
gem "importmap-rails", "~> 1.1", ">= 1.1.5"
gem "jsbundling-rails", "~> 1.0", ">= 1.0.3"
gem "pg", "~> 1.2", ">= 1.2.3"
gem "puma", "~> 5.0"
gem "rails", "~> 7.0.1"
gem "rails_semantic_logger", "~> 4.6"
gem "sprockets-rails", "~> 3.4", ">= 3.4.2"
gem "stimulus-rails", "~> 1.1"
gem "turbo-rails", "~> 1.1", ">= 1.1.1"
gem "tzinfo-data", "~> 1.2021", ">= 1.2021.1"

# ASSETS #

group :development, :test do
  gem "byebug", "~> 11.1", ">= 11.1.3"
  gem "rails-controller-testing", "~> 1.0"
  gem "rspec", "~> 3.10"
  gem "rspec-rails", "~> 5.0"
end

group :development do
  gem "annotate", "~> 3.2"
  gem "brakeman", "~> 5.0", require: false
  gem "bullet", "~> 7.0", ">= 7.0.3"
  gem "bundle-audit", "~> 0.1.0"
  gem "listen", "~> 3.5", ">= 3.5.1"
  gem "rubocop", "~> 1.12", ">= 1.12.1", require: false
  gem "rubocop-performance", "~> 1.11"
  gem "rubocop-rails", "~> 2.9", ">= 2.9.1"
  gem "rubocop-rspec", "~> 2.4"
  gem "rubocop-shopify", "~> 2.1"
  gem "solargraph", "~> 0.40.4"
  gem "spring", "~> 2.1", ">= 2.1.1"
end
