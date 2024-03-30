task :default => :proposal
task :proposal => "build/proposal.pdf"

directory "build"

file "build/proposal.pdf" => ["build", "proposal/index.md"] do
  sh "pandoc -f markdown -t pdf -o build/proposal.pdf proposal/index.md"
end
