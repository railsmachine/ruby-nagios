require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "ruby-nagios"
    gem.version = "0.1.0"
    gem.summary = %Q{CLI and Ruby library for querying nagios services status}
    gem.description = %Q{
Have you ever had to disable alerts, retry a check or acknowledge outages on a large amount of services with Nagios and hated the web UI for it?

This is a CLI tool and Ruby library that parses your status log file and let you query it for information or create external commands to be piped into the nagios command file. 
}
    gem.email = "rip@devco.net"
    gem.homepage = "http://code.google.com/p/ruby-nagios/"
    gem.authors = ["R.I.Pienaar"]
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

require 'rake/rdoctask'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = "ruby-nagios #{version}"
  rdoc.rdoc_files.include('README*')
  rdoc.rdoc_files.include('lib/**/*.rb')
end
