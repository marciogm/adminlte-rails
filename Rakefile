require 'rake'
require 'fileutils'

task :update_javascripts
  Dir.glob('AdminLTE/plugins/**/*.js').each do |file|
    dir, filename = File.dirname(file), File.basename(file)
    dest = File.join("vendor/assets/javascripts", dir)
    puts "#{dest}/#{filename}"
    # FileUtils.mkdir_p(dest)
    # FileUtils.copy_file(file, File.join(dest,filename))
end


task :update_stylesheets
  Dir.glob('AdminLTE/plugins/**/*.css').each do |file|
    dir, filename = File.dirname(file), File.basename(file)
    dest = File.join("vendor/assets/stylesheets", dir)
    FileUtils.mkdir_p(dest)
    FileUtils.copy_file(file, File.join(dest,filename))
end


task :update_png
  Dir.glob('AdminLTE/plugins/**/*.png').each do |file|
    dir, filename = File.dirname(file), File.basename(file)
    dest = File.join("vendor/assets/stylesheets", dir)
    FileUtils.mkdir_p(dest)
    FileUtils.copy_file(file, File.join(dest,filename))
end

task :copy_dist
end
