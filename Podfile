platform :ios, '12.0'

target 'HDWalletKit' do
    use_frameworks!
    pod 'secp256k1.swift', '~> 0.1.4'
    pod 'CryptoSwift', '~> 1.0.0'

    target 'HDWalletKit_Tests' do
        pod 'CryptoSwift', '~> 1.0.0'
	pod 'secp256k1.swift', '~> 0.1.4'
    end
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
    end
  end
end
