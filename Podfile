platform :ios, '10.0'

use_frameworks!

swift_version = "4.0"

target 'WireGuard' do
  pod 'SwiftLint'
  pod 'PromiseKit/CorePromise'
  pod 'Disk'
  pod 'BNRCoreDataStack'

  post_install do | installer |
    require 'fileutils'
    FileUtils.cp_r('Pods/Target Support Files/Pods-WireGuard/Pods-WireGuard-acknowledgements.plist', 'Resources/Settings.bundle/Acknowledgements.plist', :remove_destination => true)

  end
end

