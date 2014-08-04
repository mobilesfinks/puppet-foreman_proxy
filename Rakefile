require 'puppetlabs_spec_helper/rake_tasks'
require 'puppet-lint/tasks/puppet-lint'

PuppetLint.configuration.log_format = '%{path}:%{linenumber}:%{KIND}: %{message}'
PuppetLint.configuration.fail_on_warnings = true
PuppetLint.configuration.send("disable_class_inherits_from_params_class")
PuppetLint.configuration.send("disable_80chars")

task :default => [:validate, :spec, :lint]
