require 'rake/clean'

file "Tyler_Roscoe_-_Resume.txt" => "Tyler_Roscoe_-_Resume.html" do
  puts "Generating Tyler_Roscoe_-_Resume.txt from Tyler_Roscoe_-_Resume.html..."
  `w3m -dump Tyler_Roscoe_-_Resume.html -cols 72 > Tyler_Roscoe_-_Resume.txt`
end

file "references.txt" => "references.html" do
    puts "Generating references.txt from references.html..."
    `w3m -dump references.html -cols 72 > references.txt`
end

desc "Generate .txt from .html. (DEFAULT)"
task :txt => ["Tyler_Roscoe_-_Resume.txt", "references.txt"]
CLEAN.include("Tyler_Roscoe_-_Resume.txt", "references.txt")

task :default => [:txt]
