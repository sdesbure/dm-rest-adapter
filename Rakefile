require 'rubygems'
require 'rake'

begin
  gem 'jeweler', '~> 1.4'
  require 'jeweler'

  Jeweler::Tasks.new do |gem|
    gem.name        = 'dm-rest-adapter'
    gem.summary     = 'REST Adapter for DataMapper'
    gem.description = gem.summary
    gem.email       = 'scott.burton [a] joyent [d] com'
    gem.homepage    = 'http://github.com/datamapper/%s' % gem.name
    gem.authors     = [ 'Scott Burton @ Joyent Inc' ]
    gem.has_rdoc    = 'yard'

    gem.rubyforge_project = 'datamapper'

    gem.add_dependency 'dm-core',       '~> 1.0.2'
    gem.add_dependency 'dm-serializer', '~> 1.0.2'

    gem.add_development_dependency 'rspec',          '~> 1.3'
    gem.add_development_dependency 'dm-validations', '~> 1.0.2'
    gem.add_development_dependency 'fakeweb',        '~> 1.3'
  end

  Jeweler::GemcutterTasks.new

  FileList['tasks/**/*.rake'].each { |task| import task }
rescue LoadError
  puts 'Jeweler (or a dependency) not available. Install it with: gem install jeweler'
end
