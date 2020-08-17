
desc "Run build task"
task :default => :build

desc "Build book"
task :build => [:clean] do
    build_dir = "build"

    sh "asciidoctor -D #{build_dir}/ -o deutschland-extrem.html deutschland-extrem.adoc"
#    cp_r 'images', "#{build_dir}/#{filename}"
end

desc "Clean build dir"
task :clean do
  rm_r Dir['build/*']
end

