require 'rake/testtask'

Rake::TestTask.new(:unit_test) do |t|
  t.libs << "test"
  t.test_files = FileList['test/unit/test_*.rb']
  t.verbose = true
end

Rake::TestTask.new(:integration_test) do |t|
  t.libs << "test"
  t.test_files = FileList['test/integration/test_*.rb']
  t.verbose = true
end

task :test => [:unit_test, :integration_test]

task :default => :test
