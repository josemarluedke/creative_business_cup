# A sample Guardfile
# More info at https://github.com/guard/guard#readme

guard 'livereload', port: '35729', host: '127.0.0.1' do
  watch(%r{app/views/.+\.(erb|haml|slim)})
  watch(%r{app/helpers/.+\.rb})
  watch(%r{public/.+\.(css|js|html)})
  watch(%r{config/locales/.+\.yml})
  # Rails Assets Pipeline
  watch(%r{(app|vendor)/assets/\w+/(.+\.(css|js|html|sass)).*})  { |m| "/assets/#{m[2]}" }
end