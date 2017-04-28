# frozen_string_literal: true

require 'bundler/gem_tasks'

task :default => %i[spec rubocop]

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec)

require 'rubocop/rake_task'
RuboCop::RakeTask.new(:rubocop)

desc 'Run benchmark'
task :benchmark do
  sh 'ruby', 'benchmark/proxy.rb'
end
