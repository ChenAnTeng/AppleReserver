platform :osx, '10.11'

target 'AppleReserver' do
  use_frameworks!
  pod 'Alamofire'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '4.0'
        end
    end
end
