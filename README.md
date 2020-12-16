# README
For repro of https://github.com/alphagov/govuk_publishing_components/pull/1831

## Requirements
- Ruby 2.7.2
- Bundler

## Setup
- Run `bundle install`
- Run `rails s`
- Observe deprecation message in log/development.log

## Validation of fix
- Uncomment second half of line 54 of Gemfile
- Run bundle install
- Clear log/development.log
- Run `rails s`
- Observe that no deprecation message is generated in log/development.log