# Uncomment the next line to define a global platform for your project
platform :ios, '14.0'

target 'CarroDemo' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  use_modular_headers!

  # Pods for CarroDemo
    pod 'IQKeyboardManagerSwift'

  target 'CarroDemoTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'CarroDemoUITests' do
    # Pods for testing
  end

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      if config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'].to_f < 14.0
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '14.0'
      end
    end
  end
end
