source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/Artsy/Specs.git'

platform :ios, '8.0'
inhibit_all_warnings!

xcodeproj 'MyProject'

  pod 'TestWithoutVersion'
pod   'TestWithVersion', '~> 0.5'
pod 'TestWith+Plus'
pod 'TestWith+PlusAndVersion'  , '~> 1.0'
pod 'TestWith/Slash'
pod 'TestWith/SlashAndVersion', '~> 0.8'
pod 'TestWithSubspecs', :subspecs => ['Bridge', 'QuerySet']
pod   'TestWithSubspecsAndVersion', '~> 0.5', :subspecs => ['Bridge', 'QuerySet']

target :test do
    pod 'TestPath', :path => '~/Documents/AFNetworking'
    pod 'TestPathAndVersion', '0.7', :path => '~/Documents/AFNetworking'
    pod 'TestGit', :git => 'https://github.com/gowalla/AFNetworking.git'
    pod 'TestGitAndVersion', '0.6', :git => 'https://github.com/gowalla/AFNetworking.git'
    pod 'TestGitBranch', :git => 'https://github.com/gowalla/AFNetworking.git', :branch => 'dev'
    pod 'TestGitBranchAndVersion', '0.5', :git => 'https://github.com/gowalla/AFNetworking.git', :branch => 'dev'
    pod 'TestGitTag', :git => 'https://github.com/gowalla/AFNetworking.git', :tag => '0.7.0'
    pod 'TestGitTagAndVersion', '0.4', :git => 'https://github.com/gowalla/AFNetworking.git', :tag => '0.7.0'
    pod 'TestGitCommit', :git => 'https://github.com/gowalla/AFNetworking.git', :commit => '082f8319af'
    pod 'TestGitCommitAndVersion', '1.2', :git => 'https://github.com/gowalla/AFNetworking.git', :commit => '082f8319af'
end

pod 'TestWithPodspec', :podspec => 'https://example.com/JSONKit.podspec'
pod 'TestWithPodspecAndVersion', '3.2', :podspec => 'https://example.com/JSONKit.podspec'

post_install do |installer|
    installer.pods_project.targets.each do |target|
        puts target.name
    end
end