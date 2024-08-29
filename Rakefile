require "asciidoctor"

task default: %i[build]

desc "Create the html directory"
directory "html"

desc "Build the macports guide"
task build: [:html] do
  Asciidoctor.convert_file 'guide/index.adoc', safe: :safe, to_file: 'html/index.html'
end
