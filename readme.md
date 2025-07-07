xcodebuild -project Unity-iPhone.xcodeproj \
  -scheme Unity-iPhone \
  -configuration Release \
  -archivePath build/UnityApp.xcarchive \
  archive


  xcodebuild -exportArchive \
  -archivePath build/UnityApp.xcarchive \
  -exportOptionsPlist ExportOptions.plist \
  -exportPath build/ipa-output
