require 'rubygems'
require 'bundler/setup'

require 'spec/rake/spectask'
require 'rcov/rcovtask'
require 'yard'

Spec::Rake::SpecTask.new(:spec) do |t|
  t.spec_files = FileList['spec/**/*_spec.rb']
  t.verbose = true
end

Rcov::RcovTask.new(:rcov) do |t|
  t.test_files = FileList['spec/**/*_spec.rb']
  t.rcov_opts  = ['--exclude', '/gems/,spec']
  t.verbose = true
end

YARD::Rake::YardocTask.new(:yard)
