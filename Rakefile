COLORFILES = {
  :vim => ['candiercode.vim', '~/.vim/colors']
}

task :default do
  COLORFILES.each do |name, files|
    `cp #{files[0]} #{files[1]}`
    puts "#{files[0]} installed to #{files[1]}"
  end


  puts "

  You'll have to manually re-import the color scheme for iTerm2:

  * open iTerm 2
  * go to iTerm > Preferences > Profiles > Colors > Load Presets
  * Browse to this directory (#{File.dirname(__FILE__)}) and choose candiercode.itermcolors

  "
end
