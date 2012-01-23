require 'rake/clean'
CLEAN.include("hireme.txt")

file "hireme.txt" => "hireme.html" do
    `w3m -dump hireme.html -cols 72 > hireme.txt`
end
