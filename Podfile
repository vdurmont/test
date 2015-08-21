
source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/Artsy/Specs.git'

platform :ios, '8.0'
inhibit_all_warnings!

xcodeproj 'MyProject'

pod    'ObjectiveSugar', '~> 0.5'
pod 'Artsy+UILabels'  , '~> 1.0'

target :test do
    pod 'AFNetworking'
    pod 'OCMock',   '~> 2.0.1'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        puts target.name
    end
end
