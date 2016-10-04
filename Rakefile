require 'rake/clean'

file "hireme.txt" => "hireme.html" do
    puts "Generating hireme.txt from hireme.html..."
    `w3m -dump hireme.html -cols 72 > hireme.txt`
end

file "references.txt" => "references.html" do
    puts "Generating references.txt from references.html..."
    `w3m -dump references.html -cols 72 > references.txt`
end

desc "Generate .txt from .html. (DEFAULT)"
task :txt => ["hireme.txt", "references.txt"]
CLEAN.include("hireme.txt", "references.txt")

task :default => [:txt]
