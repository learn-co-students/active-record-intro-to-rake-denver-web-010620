namespace :greeting do
  desc 'oputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
  
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end
end

desc 'drops into console'
task :console => :environment do
end

namespace :db do
  task :environment do
    require_relative './config/environment'
  end
  
  task :migrate => :environment do
    Student.create_table
  end

  task :seed do
    require_relative './db/seeds.rb'
  end
end
