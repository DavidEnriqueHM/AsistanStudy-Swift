platform :ios, '10.0'

target 'AsistanStudy' do
    pod 'BMSCore', '~> 2.0'




    # Comment this line if you're not using Swift and don't want to use dynamic frameworks

    use_frameworks!

    pod 'MessageKit', '~> 0.13'
    pod 'IBMWatsonAssistantV1', '~> 1.3.1'
    pod 'NVActivityIndicatorView'

    post_install do |installer|
        installer.pods_project.targets.each do |target|
            if ['SwiftCloudant'].include? target.name
                target.build_configurations.each do |config|
                    config.build_settings['SWIFT_VERSION'] = '3.2'
                end
            end
        end
    end
    # Pods for AsistanStudy
    target 'AsistanStudyTests' do
        inherit! :search_paths
        # Pods for testing
    end

    target 'AsistanStudyUITests' do
        inherit! :search_paths
        # Pods for testing
    end

end
