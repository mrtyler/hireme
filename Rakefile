require 'rake/clean'

file "hireme.txt" => "hireme.html" do
    puts "Generating hireme.txt from hireme.html..."
    `w3m -dump hireme.html -cols 72 > hireme.txt`
end
desc "Generate hireme.txt from hireme.html. (DEFAULT)"
task :txt => ["hireme.txt"]
CLEAN.include("hireme.txt")

task :default => [:txt]
