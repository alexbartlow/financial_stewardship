
task :generate do
  puts `asciidoc -a toc -a stylesheet=~/Projects/financial_stewardship/stylesheets/scribe.css -o output/book.html book/book.asc`
end

task :wc do
  puts `wc -w book/*.asc`
end

task :publish => [:generate] do
  `cp output/book.html ~/Dropbox/Public/financial_stewardship.html`
end
