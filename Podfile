# Uncomment the next line to define a global platform for your project
platform :ios, '14.0'
install! 'cocoapods', :disable_input_output_paths => true

target 'CarroDemo' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  use_modular_headers!

  # Pods for CarroDemo
  pod 'IQKeyboardManagerSwift'
  pod 'EmptyDataSet-Swift'
  pod "ESPullToRefresh"
  pod 'TLPhotoPicker'
#  pod 'Alamofire'
#  pod 'AlamofireImage', '~> 3.5'
  pod 'SnapKit'
  pod 'PromiseKit', '~> 6.8'
  pod 'Swinject'
  pod 'KeychainAccess'
  pod 'FMDB'
  pod 'Siren'
#  pod 'Firebase/Core'
#  pod 'Firebase/Messaging'
#  pod 'Firebase/Auth'
#  pod 'Firebase/RemoteConfig'
  pod 'Sentry'
  
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
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '14.0'
    end
  end
end
