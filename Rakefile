desc "Run the test suite"

task :test do
  build = "xcodebuild \
    -workspace UIViewDraggableDemo/UIViewDraggableDemo.xcworkspace \
    -scheme UIViewDraggableDemo \
    -sdk iphonesimulator -destination 'platform=iOS Simulator,name=iPhone 6,OS=9.2'"
  system "#{build} test | xcpretty --test --color"  
end

task :default => :test
