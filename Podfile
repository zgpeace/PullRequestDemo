# Uncomment the next line to define a global platform for your project
platform :ios, '12.2'

target 'KnobShowcase' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for KnobShowcase
  pod 'KnobControl', :git => 'https://github.com/zgpeace/KnobControl.git', :tag => '1.0.1'
end

# Workaround for Cocapods issue #7606
post_install do |installer|
	installer.pods_project.build_configurations.each do |config|
		config.build_settings.delete('CODE_SIGNING_ALLOWED')
		config.build_settings.delete('CODE_SIGNING_REQUIRED')
	end
end
