inhibit_all_warnings!
use_frameworks!

target 'WatchButton' do

end

target 'WatchButton WatchKit Extension' do

pod 'ContentfulDeliveryAPI'

end

# Because AFNetworking internally uses `sharedApplication`
post_install do |installer|
  installer.project.targets.each do |target|
    target.build_configurations.each do |config|
    	config.build_settings['APPLICATION_EXTENSION_API_ONLY'] = 'NO'
    end
  end
end
