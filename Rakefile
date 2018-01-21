task :deploy do
  desc 'Build and deploy site to skylar.anderson.is'

  system('bundle exec middleman build')
  system('gsutil -h "Cache-Control:public,max-age=3600" cp -a public-read -r build/* gs://skylar.anderson.is')
end


